class I_am( ):
    
    def __init__( self ):
        self.name = "Michael"
        self.age = 23
        self.city = "Guarabira"
        self.state = "PB"
        self.country = "Brazil"

    def description( self ):
        return "%s, %d age, live-in city %s, %s - %s" %(self.name, self.age, self.city, self.state, self.country)

class Skills( ):
    
    def __init__( self ):
        self.language = ["Python", "Java", "JS", "R", "NodeJs", "Django", "SQLite", "Postgresql", "MongoDB", "MEMES"]
     
    def michael( self ):
        michael = I_am()
        out = michael.description()
        return out
    
    def list_skills( self ):
        string_out = self.michael() + ", experience with -> "
        for i in self.language:        
            string_out += i + " - "              
        return string_out

michael_print = Skills()        
print(michael_print.list_skills())
