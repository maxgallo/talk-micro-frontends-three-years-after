# [fit] Micro-frontends,
### [fit] **three years after**

<br />
<br />
<br />

### @**_maxgallo**

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

[.column]
<br><br><br><br><br><br>
# [fit] Agenda

[.column]
<br><br><br>
# 🂡 __Three Years Ago__
# 🂢 __Three Challenges__
# 🂣 __Three Takeaways__

---
# [fit] Three Years Ago 
# __Three Challenges__
# __Three Takeaways__
<br />
<br />
<br />
### @**_maxgallo**

---

[.column]

<br><br>
# [fit] DAZN
# [fit] Three Years Ago

[.column]
<br><br><br><br><br>
## ☞ __Live Sport Streaming__
## ☞ __Rapid Growth__
## ☞ __~6 Frontend teams__

---

# [fit] __2018__ Frontend Architecture


![original 50%](./images/monolith_vs_vertical_mfes.png)


^ 6 Vertical MFE (catalog, auth, landingpage, help, myaccount, error)
^ Bootstrap: clientside orchestrator
^ Not a single line of code shared
^ Autonomous teams

---

# [fit] __Micro-frontends:__ Vertical vs Horizontal


![original 48%](./images/vertical_horizontal.png)


^ 6 Vertical MFE (catalog, auth, landingpage, help, myaccount, error)
^ Bootstrap: clientside orchestrator
^ Not a single line of code shared
^ Autonomous teams

---

# [fit] __2018__ Runtime Frontend Architecture


![original 60%](./images/bootstrap.png)


^ 6 Vertical MFE (catalog, auth, landingpage, help, myaccount, error)
^ Bootstrap: clientside orchestrator
^ Not a single line of code shared
^ Autonomous teams

---

# __Three Years Ago__ 
# [fit] Three Challenges
# __Takeaways__
<br />
<br />
<br />
### @**_maxgallo**

---

__Challenge #1: Boundaries Definition__
<br><br><br><br>
# __Some vertical Micro-frontends were__ too big __for a single team.__

![right 58%](./images/too_many_teams.png)

^ Release Trains
^ Cross-teams coordination needed

<br><br><br><br><br><br><br><br><br><br>

@**_maxgallo**

---

# __Solution #1__ Re-define boundaries

![original 55%](./images/vertical_split.png)

^ Runtime Approach doesn't change, there's always one team in every view

---

# __Vertical Micro-Frontend,__ Ownership is at least a page.


---

# [fit] __Solution #2__ Horizontal Micro-Frontends

![original 55%](./images/solution2.png)


^ systemJS wrapper
^ Comparison: Module Federation or Single-SPA ?

---

[.column]
<br><br><br><br><br>
# [fit] Deep Dive
## [fit] Horizontal Micro-frontends

[.column]
<br>

## ☞ __Multiple Teams owning parts of the same page__
## ☞ __Coordination needed__
## ☞ __Independent Releases__


^ Example: complex subsystem (Team topologies): playback

---

# Deep Dive
## __Horizontal Micro-frontends__
## __in__ DAZN

![original 50%](./images/horizontal_microfrontends_dazn.png)

^ Wrapper Around SystemJS
^ Breaking Changes releases (major in semver) are blocked by host
^ Other releases (Minor & patch) are owned by team

---

__Challenge #2: Beyond Team Autonomy__
<br><br><br><br>
# __Teams were autonomous, but creating__ silos.

![right 45%](./images/team_silos.png)

^ How to spot the signs
^ Principal Engineers or cross team tech people

<br><br><br><br><br><br><br><br><br><br>

@**_maxgallo**

---

[.column]

# Share Knowledge
<br><br><br><br><br>
### __☞__ Frontend Guilds


[.column]

# __Decide Together__
<br><br><br><br><br>
### __☞ Request For Comments (aka RFC)__


[.column]

# Discover <br>More
<br><br><br><br><br>
### ☞ Backstage (Spotify)

---

__Challenge #3: To Share, or not to Share__
<br>
# __There are__ visual inconsistencies __, but not a single visual component has been shared across all the Micro-frontends,__ yet.

![right 45%](./images/share.png)

^ it's been not easy how "not share" was helping deliver faster
^ New Phase soon (company is more mature)
^ something currently shared: payments (business critical)

<br><br>

@**_maxgallo**

---

# __Three Years Ago__ 
# __Three Challenges__
# [fit] Three Takeaways
<br />
<br />
<br />
### @**_maxgallo**
---

# [fit] Three Takeaways

  - Re evaluate your decisions, and keep Decision Records
  - Think about sharing but don't use "number of shared components" as metric
  - It's always about people

---


#[fit] Thank You


# [fit] **github.com/maxgallo/talk-micro-frontends-three-years-after**

<br />
<br />
<br />

### @**_maxgallo**
