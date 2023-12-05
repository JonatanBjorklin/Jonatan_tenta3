# Jonatan_tenta3
NodeJs/Prisma/MySQL Tenta

1. Kan du förklara skillnaden mellan synkron och asynkron kod i Node.js?
I en synkron programmeringsmodell så körs varje kodade efter att föregående kodrad är avslutad. Man kan läsa koden uppifrån och ned och få en känsla för den ordning som koden exekveras i. 

I en asynkron programmeringsmodell, vilken också kan benämnas med Asynchronous I/O, så finns det en central event loop som styr exekveringen. Så fort en operation, en kodrad, blockar på I/O, så lämnas exekveringskontrollen över till event loopen. Detta sker till exempel när vi låter användaren mata in något från tangentbordet, eller när vi läser och skriver till filer. Dessa är blockande operationer.

2. Beskriv användningen av middleware i Express och ge exempel på några vanliga
middleware.
Middleware hjälper till med att organisera och strukturera hanteringen av förfrågningar och svar i Express-applikationer. Det ger en flexibel och modulär arkitektur som underlättar utvecklingen och underhållet av webbapplikationer.

3. Vilka fördelar erbjuder Prisma när det gäller att interagera med databasen?
Prisma erbjuder Migrations, Active Maintenance, Support for DB of your choice när det gäller att integrera med databasen.
4. Hur definierar du en modell för en tabell i Prisma?
Man skriver in model namnPåTabellen och sen i {} så skriver man in vad man vill ska va i tabellen och sen lägger man sen vad som man vill ha till sin tabell. 
model User {
  id      Int      @id @default(autoincrement())
  username   String   @unique
  password    String?
  roll Boolean @default(false)
}

5. Vad är skillnaden mellan npm install och npm install --save?
Npm install så installerar man till hela enheten och alla mappar och allt får det man installerar, men när man skriver npm install --save så installerar man just till en specifik mapp.
