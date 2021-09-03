# Location

## Choose the best location estimate

**The FusedLocationProviderClient provides several methods to retrieve device location information. Choose from one of the following, depending on your app's use case:**

- ***getLastLocation() gets a location estimate more quickly and minimizes battery usage that can be attributed to your app. However, the location information might be out of date, if no other clients have actively used location recently.***

- ***getCurrentLocation() gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device***

    ***This is the recommended way to get a fresh location, whenever possible, and is safer than alternatives like starting and managing location updates yourself using requestLocationUpdates(). If your app calls requestLocationUpdates(), your app can sometimes consume large amounts of power if location isn't available, or if the request isn't stopped correctly after obtaining a fresh location.***
