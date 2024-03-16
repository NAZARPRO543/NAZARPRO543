class Human:
    def __init__(self, name="Human"):
        self.name = name
class Auto:
        def __init__(self, brand):
           self.brand = brand
           self.passengers = [] #список
        def add_passenger(self, human):
            self.passengers.append(human)
        def add_passenger(self, *args):
            for passenger in args:
                self.passengers.append(passenger)
        def print_passengers_names(self):
            if self.passengers!= []:
                print(f"Names of {self.brand} passengers:")
                for passenger in self.passengers:
                 print(passenger.name)
            else:
                print(f"There are no passengersin {self.brand}")

Nazar = Human("Nazar") #екземпляр класу (об'єкт)
Danya = Human("Danya") #екземпляр класу (об'єкт)
car = Auto("Mercedes") #екземпляр класу (об'єкт)

car.add_passenger(Nazar)  #зв'язок класів
car.add_passenger(Danya)
car.print_passengers_names()
