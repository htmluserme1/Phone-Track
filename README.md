import phonenumbers
from phonenumbers import timezone
from phonenumbers import geocoder
from phonenumbers import carrier

#enter phone number along with country
number= input("+9779865057511:")

#Parsing String to the Phone number
phoneNumber = phonenumbers.parse(9865057511)

#printing the timezone using the timezone module
timezone = timezone.time_zone_for_number(9865057511)
print("timezone : "+str(timezone))

# printing the geolocation of the given number using the geocoder module
geolocation = geocoder.description_for_number(9865057511,"en")
print("location : "+geolocation)

setvice = carrier.name_for_number(9865057511,"en")
print("service provider : "service)
