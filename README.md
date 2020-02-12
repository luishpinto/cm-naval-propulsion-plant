# Condition Based Maintenance of Naval Propulsion Plants Data Set

**Abstract:** Data have been generated from a sophisticated simulator of a Gas Turbines (GT), mounted on a Frigate characterized by a COmbined Diesel eLectric And Gas (CODLAG) propulsion plant type.

**Source:**

Andrea Coraddu(2), Luca Oneto(1), Alessandro Ghio(1), Stefano Savio(2), Davide Anguita(3), Massimo Figari(2)

1. Smartlab -- Non-Linear Complex Systems Laboratory | DITEN - Università degli Studi di Genova, Genoa (I-16145), Italy.
2. Marine Technology Research Team | DITEN - Università degli Studi di Genova, Genoa (I-16145), Italy.
3. Smartlab -- Non-Linear Complex Systems Laboratory.
4. DIBRIS -- Università degli Studi di Genova, Genoa (I-16145), Italy.

cbm@smartlab.ws

www.cbm.smartlab.ws

## Data Set Information:

The experiments have been carried out by means of a numerical simulator of a naval vessel (FRIGATE) characterized by a gas turbine (GT) propulsion plant. The different blocks forming the complete simulator (propeller, hull, GT, gear box and controller) have been developed and fine tuned over the year on several similar real propulsion plants. In view of these observations the available data are in agreement with a possible real vessel.

In this release of the simulator it is also possible to take into account the performance decay over time of the GT components such as GT compressor and turbines.

The propulsion system behaviour has been described with this parameters:
- ship speed (linear function of the lever position lp).
- compressor degradation coefficient kMc.
- turbine degradation coefficient kMt.

so that each possible degradation state can be described by a combination of this triple (lp, kMt, kMc).
The range of decay of compressor and turbine has been sampled with an uniform grid of precision 0.001 so to have a good granularity of representation.

In particular for the compressor decay state discretization the kMc coefficient has been investigated in the domain [1; 0.95], and the turbine coefficient in the domain [1; 0.975].

Ship speed has been investigated sampling the range of feasible speed from 3 knots to 27 knots with a granularity of representation equal to tree knots.

A series of measures (16 features) which indirectly represents of the state of the system subject to performance decay has been acquired and stored in the dataset over the parameter's space.

Check the README.txt file for further details about this dataset.

## Attribute Information:

A 16-feature vector containing the GT measures at steady state of the physical asset:

Feature | Variable | Unit
--------|----------|-----
lever position | lp |
ship speed | v | knots
gas Turbine (GT) shaft torque | GTT | kN m
GT rate of revolutions | GTn | rpm
gas generator rate of revolutions | GGn | rpm
starboard propeller torque | Ts | kN
port propeller torque | Tp | kN
hight pressure (HP) turbine exit temperature | T48 | °C
GT compressor inlet air temperature | T1 | °C
GT compressor outlet air temperature | T2 | °C
HP turbine exit pressure | P48 | bar
GT compressor inlet air pressure | P1 | bar
GT compressor outlet air pressure | P2 | bar
GT exhaust gas pressure | Pexh | bar
turbine injecton control | TIC | %
fuel flow | mf | kg/s
GT compressor decay state coefficient | kMc |
GT turbine decay state coefficient | kMt |
