# [fit] Micro-frontends
### [fit] **three years after**

<br />
<br />
<br />

### @**_maxgallo**

---

## __In 2019 I was on this stage with__ Luca Mezzalira __to introduce DAZN approach to__ Micro-frontends

![right fill filtered](./images/max_luca.JPG)

^ March 2019
^ Incredible response / feedback / questions

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
https://bit.ly/talk-max-luca

---

# [fit] Hi 👋 I'm Max

### 🇮🇹 🇬🇧 🍝 💻 🎶 🏍 📷 ✈️ ✍️

### **Principal Engineer @ DAZN**

<br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

### twitter: @**_maxgallo**
### web: **maxgallo.io**

![right 30%](./images/me.png)

---

<!--

Intro
    - DAZN Context
        - Product
        - Number of teams
    - Three Years ago
        - 6 Vertical MFE (catalog, auth, landingpage, help, myaccount, error)
        - Bootstrap: clientside orchestrator
        - Not a single line of code shared
        - Autonomous teams

Challenges
  - Vertical MFE where too big
    - How to spot the signs
        - release trains
        - cross teams coordination needed
    - What we put in place
        - systemJS wrapper
        - Comparison: Module Federation or Single-SPA ?
  - Extreme of autonomy -> Silo
    - How to spot the signs
        - Principal Engineers or cross team tech people
    - What to put in place
        - FE Guilds
        - RFC
        - Service Discovery: Backstage
  - Sharing: is it a problem?
    - Visual Inconsistencies
    - What are we sharing
        - payments
        - experiments
        - payments
Takeaways
  - Re evaluate the decisions (And keep Decision Records)
  - Think about sharing but don't use "number of shared components" as metric
  - aaaaa

-->

# Agenda

## ☞ __Once Upon a Time__
## ☞ __Domain Boundaries Evolution__
## ☞ __Beyond Team Autonomy__
## ☞ __Sharing Code__

---


![original fit](./images/book_1.png)

[.column]
# [fit] __Once Upon a Time__
### Part 1 of 4

[.column]
<br>

---

# __Once Upon a Time, there was a Live Sport Streaming Company called__ DAZN

![right 45%](./images/football.png)

---

![original 50%](./images/growth.png)

[.column]
# __DAZN Engineering department was growing__ exponentially

[.column]
<br>

---

# __To sustain our teams growth plans so we introduced__ Micro-frontends


![right 50%](./images/monolith_vs_vertical_mfes.png)

---

# [fit] __DAZN Micro-frontends__ Manifesto

### ☞ __Modelled around a Business Subdomain__
### ☞ __Independent implementation__
### ☞ __Owned by a single team__
### ☞ __Entire view__

<br><br><br><br><br>
### @**_maxgallo**

![original 50%](./images/manifesto.png)

<!--

# [fit] __2018__ Runtime Frontend Architecture


![original 60%](./images/bootstrap.png)


^ 6 Vertical MFE (catalog, auth, landingpage, help, myaccount, error)
^ Bootstrap: clientside orchestrator
^ Not a single line of code shared
^ Autonomous teams
-->

---
...and they lived happily ever after

---

...and they lived happily ever after
#[fit] __Nope!__

---

![original fit](./images/book_2.png)

[.column]
# [fit] __Domain Boundaries Evolution__
### Part 2 of 4

[.column]
<br>

---


# __It's not easy to define__ Domain Boundaries

![right 80%](./images/subdomain_evolution.gif)

---


![original 55%](./images/too_many_teams.png)

[.column]
# __Some vertical Micro-frontends were__ too big __for a single team__

^ Release Trains
^ Cross-teams coordination needed
^ Evolution of the boundaries

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### @**_maxgallo**

[.column]
<br>

---
# __Our business subdomains are not immutable so we re-defined their__ boundaries

![right 65%](./images/vertical_split.png)

^ We merged microfrontends
^ Runtime Approach doesn't change, there's always one team in every view
^ there are limits for this

---

# __A Subdomain did contain a complex subsystem[^1] that__ was not considered a Micro-frontend
![right 65%](./images/single_view.png)

[^1]: From "Team Topologies"

^Ownership is at least a page.
^If we step back a second, going high level

---

# [fit] __Micro-frontends__ Vertical & Horizontal[^2] split


![original 48%](./images/vertical_horizontal.png)

[^2]: Module Federation, Single SPA

---
<!--
[.column]
# __Deep Dive into__ Horizontal Micro-frontends

[.column]
<br>

## ☞ __Multiple Teams owning parts of the same view__
## ☞ __Coordination needed__
## ☞ __Independent Releases__

---
-->

![original 50%](./images/horizontal_microfrontends_dazn.png)

[.column]
# __Deep Dive into Horizontal Micro-frontends in__ DAZN
<br><br><br><br>
☞ SystemJS
☞ Relationship with host
☞ Autonomy in non-breaking <br>changes


[.column]
<br>


^ Wrapper Around SystemJS
^ Breaking Changes releases (major in semver) are blocked by host
^ Other releases (Minor & patch) are owned by team



<!--
# [fit] __Solution #2__ Horizontal Micro-Frontends

![original 55%](./images/solution2.png)


^ systemJS wrapper
^ Comparison: Module Federation or Single-SPA ?
-->


---

![original fit](./images/book_3.png)

[.column]
# [fit] __Beyond Team Autonomy__
### Part 3 of 4

[.column]
<br>

---
# __Very autonomous Teams are at risk to create__ silos

![right 48%](./images/team_silos.png)

^ How to spot the signs
^ Principal Engineers or cross team tech people

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### @**_maxgallo**

---

[.column]
# __Share Knowledge__ across Teams

[.column]
<br><br><br><br><br>
## ☞ __Frontend Guilds__
## ☞ __Principals & Architects__

---

[.column]
# __Favor local decisions__ but have a plan for global decisions
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### @**_maxgallo**

[.column]
<br><br><br><br><br>
## ☞ __Request For Comments (aka RFC)__
## ☞ __Decision Records (aka ADR)__

---

# __Enable Discovery__ beyond Teams

<br><br><br><br><br>
### ☞ __Backstage (Spotify)__

![right 40%](./images/backstage.png)

---

![original fit](./images/book_4.png)

[.column]
# [fit] __Sharing Code__
### Part 4 of 4

[.column]
<br>

^ Duplicating by design

---

# __Not a single visual component has been shared across all the Micro-frontends,__ yet

![right 45%](./images/share.png)

^ Not an easy journey
^ why "visual"

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

### @**_maxgallo**

---

[.column]
# __In DAZN, we're sharing some components to reflect__ company priorities

^ New Phase soon (company is more mature)
^ something currently shared: payments (business critical)

<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
### @**_maxgallo**

[.column]
<br><br><br><br><br><br><br><br><br><br><br><br><br>

---
# __What are we sharing and__ why

<br>

[.column]
## ☞ __Payments__
Critical component

[.column]
<br>

[.column]
<br>

---

# __What are we sharing and__ why

<br>

[.column]
## ☞ __Payments__
Critical component

[.column]
## ☞ __Analytics__
Risks in duplication

[.column]
<br>

---

# __What are we sharing and__ why

<br>

[.column]
## ☞ __Payments__
Critical component

[.column]
## ☞ __Analytics__
Risks in duplication

[.column]
## ☞ __Experiments__
Hard to provide autonomy

---

# [fit] Takeaways

__☞__ Your business subdomains are _not immutable_
__☞__ Share as a _solution_ not as a _goal_
__☞__ It's always about _people_

<br><br><br><br><br>

### @**_maxgallo**
---

<br>

#[fit] Thank You


# [fit] **github.com/maxgallo/talk-micro-frontends-three-years-after**
<br>


### @**_maxgallo**

