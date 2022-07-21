# KOOMPI Fi-Fi Pilot @VitaminAir

## Motivation

The ideas is to utilize 4G internet from telco via smartphone or modem and build a mesh network to share wifi internet in the area such as VitaminAir. If it works well, then many places in the world could also use concept.

In our case, we want to tether internet from a smartphone to a KOOMPI Local Content Server, which act as the Internet receiver, then share it directly to Grandmaster AP (`access point`). 

The GrAP then share internet with other ChildAP. The ChildAP provide WiFi Internet to users.

## Internet Privider

We will try with Smart 4G cost 8 USD per month for 100 GB data.  

## Flow chart of the set up

```mermaid
graph TD
    A[4G Internet] -->|Tether| B(Content Server)
    B --> |SameLocation| C{Grandmaster AP}
    C -->|AP-#1| D[Office #1]
    D -->|AP-#2| E[Office #2]
    C --> |AP-#N| G(office #N)
    E -->|AP-#3| F[Office #3]
    
``` 
## The Site

The distant from;
- GAP to Office #1 is same location
- Office #1 - Office #2 = 30m
- Office #2 - Office #3 = 50m

The whole campus is around 120 m^2.  




