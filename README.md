```python

    class I_am():

        def __init__(self):       
            self.name = "Michael"
            self.age = 24
            self.city = "Guarabira"
            self.state = "PB"
            self.country = "Brazil"

        class Skills( ):

            def __init__(self): 
                self.languages = ["Python","Java","JS","R","TS"]
                self.frameworks = ["NodeJS","Django","Flask","Spring Boot","ReactJS"]
                self.databases = ["SQLite","MySQL","Postgresql","MongoDB"]
                self.others = ["Docker"]

        def description(self):            
            list_skills = self.Skills()      
            return "%s, %d age, live-in city %s, %s - %s" %(self.name, self.age, self.city, self.state, self.country)     

        def list_skills(self):
            list_skills = self.Skills()
            list_full = [list_skills.languages,list_skills.frameworks,list_skills.databases,list_skills.others]
            string_out = self.description() + ", experience with -> "
            for datas in list_full:
                for data in datas:
                    string_out += str(data) + " - "
            return string_out

    
    if __name__ == '__main__':
        michael_print = I_am()
        print(michael_print.list_skills())
```
