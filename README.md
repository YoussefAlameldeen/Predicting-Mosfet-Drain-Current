# Predicting-Mosfet-Drain-Current
MOSFET is a unipolar device where the current conduction mechanism takes place by the majority of carriers. A MOS transistor consists of four terminals called a drain, gate, source, and substrate. In most cases, the substrate is connected to the ground for N-channel MOSFET and to supply voltage for P-channel MOSFET. The variation in drain current takes place due to the variation in drain-source or gate-source voltage.

Commercial circuit simulator such as CADENCE uses the SPICE engine to simulate electronic circuits. While coming to VLSI level integration, millions of MOS transistors are connected together to form the chip. Since prototype development is a costly matter, before fabrication, the design is passed through several testing and simulation levels.

While talking about semiconductor device modeling, basically reflects a set of equations that describe current-voltage characteristics, capacitance, and maybe some other parameters depending upon the type of the device. For a MOS transistor, the drive current i.e. the drain current depends upon terminal voltages such as drain and gate voltages. Also, it depends upon geometry such as length, width, and material properties such as mobility, carrier velocity, etc. While developing a model, all these parameters need to be carefully considered.

There are three approaches to developing a model of any semiconductor device.

Physics-based model: They are the most accurate, they are derived by applying device physics, solving equations, etc. As a result, they are difficult to develop, time taking and sometimes they are impossible to develop especially for new devices/materials where the device physics is unknown.
Empirical model: They are based upon curve fitting using a polynomial. Due to their fitting nature, they are less accurate and might not capture the variation of any parameter properly. But they are much easier to develop. Most of the MOSFET models available so far are semi-empirical in nature.
Look-up Table approach: It is another approach for model development where the data points are stored in form of a table. The simulator will pick up the input variable and its corresponding output without solving any equations. But a large number of data points are required. Accuracy is less compared to physics-based models.
