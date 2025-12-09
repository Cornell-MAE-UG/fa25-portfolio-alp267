<img src="./nfbcicvv.png"
style="width:4.83333in;height:1.83333in" />

**ENGRD** **2020** **Updated** **Portfolio:** **Mechanism**
**Including** **an** **Actuator**

The goal of this mechanism is to maximize the height that our
machine/system can lift a weight using a linear actuator, within a fixed
space of 150 cm by 50 cm. The system is made up of two ground-mounted
pinned supports at points A and B, a rigid lifting bar, and a single
rod-type actuator. Everything is assumed to be rigid.

<u>Design Objectives:</u>

> ● Maximize vertical lift height (h)
>
> ● Maximize the allowable lifting weight (not my main goal)

<u>Constraints:</u>

> ● 150 cm x 50 cm space
>
> ● Peak actuator thrust: 35.81 kN ● Pin A Coordinates: (0,0)
>
> ● Pin B Coordinates: (120.00 cm,0) ● Bar Length: 50 cm

<u>Analysis:</u>

We will treat the bar as a rigid body and the actuator will produce a
vertical lifting reaction.

> Wmax = Factuatorsin(Θ) =

Factuator = 35.81 kN

Θ = tan-1(bar/distance between pins) = tan-1(0.5m/1.2m) = 22.62o

> Wmax = (35.81 kN)\*sin(22.62) = 13.77 kN

Therefore, the upper bound load of the rigid-body is approximately 13.77
kN.

**Step** **2:**

Now we are going to treat the bar as a beam instead of a perfectly rigid
bar. It will deflect due to the payload weight and the actuator induced
transverse load.

<u>Assumptions:</u>

> ● Small deflections
>
> ● Transverse loading only
>
> ● Simply supported between A-B
>
> ● Point load at distance 4.35 cm (or at the tip of the 50 cm bar) ●
> Material & Properties: Steel → E = 200 GPA

<u>Analysis:</u>

Find the max deflection based on the above information:

> δmax = Wb3/48EI

W = 13.77 kN and the rectangular cross section has a width of 20 mm and
a height of 40 mm.

I = bh3/12 = (0.020 m)(0.040 M)3/12 = 1.07x10-7 m4

> δmax = (13.77 kN)(0.020 m)3/48(200x109 Pa)(1.07x10-7 m4) = 0.000107 mm

<img src="./ke5ee4uf.png" style="width:6.5in;height:8.40625in" />This
works with the restrictions (I think, I’m tired 🙂)
