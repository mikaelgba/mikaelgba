README.md

    class I_am():

        def __init__(self):       
            self.name = "Michael"
            self.age = 23
            self.city = "Guarabira"
            self.state = "PB"
            self.country = "Brazil"
    
        class Skills( ):
        
            def __init__(self): 
                self.language = ["Python", "Java", "JS", "R", "NodeJS", "Django", "Flask", "SQLite", "Postgresql", "MongoDB", "MEMES"]

        def description(self):            
            list_skills = self.Skills()      
            return "%s, %d age, live-in city %s, %s - %s" %(self.name, self.age, self.city, self.state, self.country)     

        def list_skills(self):
    
            list_skills = self.Skills()
            string_out = self.description() + ", experience with -> "
            for i in list_skills.language:        
                string_out += i + " - "              
            return string_out

    
    if __name__ == '__main__':
        michael_print = I_am()
        print(michael_print.list_skills())
