# Zadanie

class RPG:
    def __init__(self,Path_of_Exile,Diablo_2):
        self.Path_of_Exile = Path_of_Exile
        self.Diablo_2 = Diablo_2

    def Torchlight_2(self):
        print("Torchlight_2 является Games")

    def Titan_Quest(self):
        print("Titan_Quest является Games")

class Tower_Defense(RPG):
    def __init__(self,Path_of_Exile,Diablo_2,Diablo_3):
        super().__init__(Path_of_Exile, Diablo_2)
        self.Diablo_3 = Diablo_3

    def Kingdom_Rush_Frontiers(self):
        print("Kingdom_Rush_Frontiers")

    def Plants_VS_Zombies(self):
        print("Plants_VS_Zombies является Tower_Defens")

class Shooter(RPG):
    def __init__(self,Path_of_Exile="default_Path_of_Exile",Diablo_2="default_Diablo_2",Diablo_3="default_Diablo_3"):
        super().__init__(Path_of_Exile, Diablo_2)
    def Call_of_Duty(self):
        print("Call_of_Duty является Shooter")

    def Battlefield_4(self):
        print("Battlefield_4 является Shooter")

a = RPG('Path_of_Exile_value','Diablo_2_value')
b = Tower_Defense('PathofExile_value','Diablo2_value','Diablo3_value')
c = Shooter()

a.Torchlight_2()
a.Titan_Quest()

b.Torchlight_2()
b.Titan_Quest()

c.Torchlight_2()
c.Titan_Quest()
c.Call_of_Duty()
c.Battlefield_4()
