# REST-Exercise
You should install the world&#39;s best air conditioner for your greenhouse. Your job is to build a REST
service with the associated REST client through which you can control and retrieve data from the air
conditioner.
The parameters to be controlled are:
• Humidity
• temperature
• Lighting
These three parameters and an additional parameter, electricity consumption over the past 24 hours,
are automatically logged every day (create files or databases, filled with relevant data, to simulate
these previous logs, you do not need to build the actual automatic logging yourself).
The functionality that your REST system needs to be able to deliver the following:
• Read the humidity right now.
• Read the temperature at the moment.
• Read the lighting right now.
• Read electricity consumption in the last 24 hours.
• Reassess the humidity
• Set new value on temperature
• Add new value to lighting
• Total report of humidity, temperature and lighting at the moment.
• Report on the humidity values, day by day, last week, end with humidity average for the week
• Report of values ​​on temperature, day by day, last week, end with temperature average for the week
• Report on the values ​​of lighting, day by day, last week, end with the average of the light for the week
• We can indicate the current electricity cost (kr / kWh) and get back the system&#39;s electricity cost for
the last week.
Additionally, you do not fully trust the built-in logging function, so for security purposes, you
will also implement functionality, by invoking a method for this, the system will log current
parameters right now to the file or database, along with a tip stamp and a note that this data
has been generated via a manual mail. Limitation: It&#39;s ok to find the values ​​of parameters
and cost, there is no requirement that they have to be realistic. Furthermore, we ignore the
delay in this task, ie. that a set value of a parameter, in reality, will differ from the actual
value of the parameter, at least for a while. When a value for a particular parameter is set, it
is the value to be read by then. Tip: Java has many classes to handle time and date,
LocalDate and LocalDateTime are the most handy to work with
In order to be approved, your solution is required to meet all of the functional requirements
above. Build a REST service that can deliver requested functionality. Also build a REST
client that calls the service&#39;s methods and displays returned data (a command client-
handler). Use files (whose data you type yourself) to persist data between program runs,
data for 8 days is enough.
