# Exercise-Teacher-Assisting

TRACCIA ESERCIZIO


Implementare ove necessario costruttori, metodi getter e setter, o altri eventuali metodi necessari.

1) Dichiarare un'interfaccia Fuel con i seguenti metodi:

 	.getEnergy(): int
   
	.refill():void

2) Dichiarare una classe astratta Vehicle con i seguenti attributi e metodi:

	.model: String

	.energy: int

		 (lancia un eccezione se maggiore di 100)
   
	.fuelType: String

   		(inizializzato come “default”)
   
	.toString

5) Dichiarare una classe GasStation con i seguenti attributi e metodi:
   
	.fuels: Map<String, Fuel>

   		(inizializzata vuota)
   
	.insertFuel(String fuelType, Fuel fuel): void

   		(aggiunge un oggetto Fuel a fuels)
   
	.rechargeStation(String fuelType): void

   		(Prende dall'HashMap l'oggetto Fuel corrispondente tramite mapkey “fuelType” e chiama il metodo refill())
   
	.chargeVehicle(Vehicle vehicle):void

    	(Prende il corretto “fuelType” dall'HashMap fuels e ricarica l'energia di vehicle tramite il metodo getEnergy())
   
8) Dichiarare le seguenti classi rappesentanti fuels:

	.Diesel con i seguenti attributi e metodi:

	.capacity: int

		inizializzata a 0

	.getEnergy(): int

		lancia un eccezione se capacity è minore o uguale a 24. Sottrae 25 all'attuale capacity e ritorna 20

	.refill(): void

		aggiunge 100 all'attuale capacity
   
	.toString

	.ChargePod con i seguenti attributi e metodi:

	.capacity: int
   
		inizializzata a 0

	.getEnergy(): int

		lancia un eccezione se capacity è minore o uguale a 19. Sottrae 20 all'attuale capacity e ritorna 15
	.refill(): void

		aggiunge 100 all'attuale capacity

	.toString

10) Dichiarare le seguenti classi rappresentanti Vehicle:

	.ElectricCar con i seguenti attributi:

	.fuelType: String

     	(inizializzata a “electric”)
    
	.DieselCar con i seguenti attributi:

	.fuelType: String

    	(inzializzata a “diesel”)
    
12) Implementare un metodo main dove:

.Un oggetto GasStation viene allocato.

.Una lista di vehicles di almeno 2 oggetti Vehicle viene allocata con all'interno almeno un oggetto ElectricCar ed un oggetto DieselCar

.Un oggetto Diesel ed un oggetto ChargePod vengono allocati ed aggiunti a GasStation tramite il metodo insertFuel

.Viene fatto il refill di tutti i fuels tramite il metodo rechargeStation

.Tutti i Vehicle all'interno della lista vehicles vengono riforniti tramite il metodo chargeVehicle di GasStation.


	



		
