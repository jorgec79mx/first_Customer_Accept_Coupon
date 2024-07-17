#Ejercicio de entrega para Modulo 5 Machine Learning
# Aqui redactaremos un resumen de lo encontrado en el ejercicio practico de si los clientes aceptarian un cupon mientras manejan

#Referencias de aprendizaje
#https://codeacademy.com/learn/learn-git

###########################################################################
# Paso 1
# Copiar la carpeta data que contiene la base coupons.csv
#
# 1. User attributes
#    -  Gender: male, female
#    -  Age: below 21, 21 to 25, 26 to 30, etc.
#    -  Marital Status: single, married partner, unmarried partner, or widowed
#    -  Number of children: 0, 1, or more than 1
#    -  Education: high school, bachelors degree, associates degree, or graduate degree
#    -  Occupation: architecture & engineering, business & financial, etc.
#    -  Annual income: less than \\$12500, \\$12500 - \\$24999, \\$25000 - \\$37499, etc.
#    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
#    -  Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
#    -  Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
#    -  Number of times that he/she eats at a restaurant with average expense less than \\$20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
#    -  Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
#
# 2. Contextual attributes
#    - Driving destination: home, work, or no urgent destination
#    - Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination
#	, and the venue, and we mark the distance between each two places with time of driving. The user can see whether 
#	the venue is in the same direction as the destination.#	
#    - Weather: sunny, rainy, or snowy
#    - Temperature: 30F, 55F, or 80F
#    - Time: 10AM, 2PM, or 6PM
#    - Passenger: alone, partner, kid(s), or friend(s)
#
#
# 3. Coupon attributes
#    - time before it expires: 2 hours or one day
############################################################################


############################################################################
# Preguntas
#
# 4. What proportion of the total observations chose to accept the coupon? 
# (data["Y"].value_counts(normalize=True)*100).round(2)
# R:	SI = 56.84%
# 	NO = 43.16%
#
# 5. Use a bar plot to visualize the `coupon` column.
# pCoupon = sns.barplot(x=data["coupon"].value_counts().index, y=data["coupon"].value_counts())
# pCoupon.tick_params(axis="x", rotation=45)
# pCoupon.set(xlabel="Categoría de Cupón", ylabel="Total")
# pCoupon.set_title("Cupones por Categoría")