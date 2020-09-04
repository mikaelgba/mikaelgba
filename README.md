class Skills( ):
    
    def __init__( self ):
        
        self.language = ["Python", "Java", "JS", "R", "NodeJS", "Django", "SQLite", "Postgresql", "MongoDB", "MEMES"]
      
    def list_skills( self ):
        
        michael = self.I_am()
        string_out = michael.description() + ", experience with -> "
        for i in self.language:        
            string_out += i + " - "              
        return string_out
    
    class I_am( ):
    
        def __init__( self ):
            
            self.name = "Michael"
            self.age = 23
            self.city = "Guarabira"
            self.state = "PB"
            self.country = "Brazil"

        def description( self ):
            
            return "%s, %d age, live-in city %s, %s - %s" %(self.name, self.age, self.city, self.state, self.country)

michael_print = Skills()        
print(michael_print.list_skills())
