@title[Inversion Of Control To Enter The Realms of Data]

@snap[west span-60]
## Inversion Of Control To Enter The Realms of Data
### Gayathri Thiyagarajan
@snapend

---

**Gayathri Thiyagarajan** <br/>
Engineering Manager @ Expedia Group <br/>
[@gaythu-rajan](https://twitter.com/gaythu-rajan)

Note:

* Java Engineer for over 15 years. I have lead many projects implementing architectures such as Microservices, Event Sourcing, CQRS. In the past year and half I have been working on delivering BigData Capture platform for one of EG brands Hotels.Com. I am avid public speaker having given many talks on Domain Driven Design. 

---

**The Context** <br/>

Note:

The product that I am going to talk about today is the Data Capture Platform that I have spearheaded for HCom in the past year or so. The objective of the platform is to many folds
1. To design and build a first party  stream of Data 
2. To overcome the challenges of the first gen Data Capture solution we had in place already
3. The solution thus built should cater different usecases for both producers and consumers

It is about the second point we will mostly talk about today

---

**First Gen Data Capture** <br/>

---

Passive data collection 
---

Less buy-in from producers
---

Data was someone else’ concern
---

Data was 2nd class citizen 

Note: 
Less focus on tooling

---
Overhead and pain

---
Changing architecture landscape

---
Details

Note:
How did we capture data then - legacy?
1. Blackbox
2. Intercept and throw data out
    1.  Captured everything - lost the meaning or essence of the data
3. Hard to debug problems and harder to roll-out fix due to integrations with dozen or so teams
4. Monitoring was a problem
    1. How do we distinguish problems at the capture level to transport level
5. Any exception seemed to point towards the library 
6. Less consideration to models - built into the library itself (lack of tooling & maturity to handle/manage schemas)
    1. Made them rigid to change
    2. Monolithic monster
    3. Loosely typed  - compromise on data quality
    
---
