# Three-Dimensional Non-Linear Finite Element Analysis [3DNLFEA]
Bambang Piscesa1, Mario M. Attard2, Ali K. Samani2

1Civil Engineering Department - Institut Teknologi Sepuluh Nopember, Surabaya 60111, East Java, Indonesia

2School of Civil and Environmental Engineering - The University of New South Wales, Sydney NSW 2052, Australia

The aim for this project is to develop three-dimensional non-linear finite element analysis for reinforced concrete structures. The project was initially started in 2014. The project is now under heavy development to improve the efficiency in the computation, as well as the stability of the program. The program is written in C# with .Net 4.6.2 platform. Several external library such as Intel MKL, Cloo.Net and ManagedCuda were integrated into the program. Up-to-date, the program is able to handle up to 100,000 hexahedral element using a computer with 16 GB memory.

# Pre and Post Processor
The program is prepared to use SALOME [1] for both the pre and post processor.

# Supported Elements
- 8-noded hexahedral element [Full (8,27 GP),Reduced (1 GP) and Selective (BBar-Element) Integrations are supported]
- 20-noded hexahedral element  [Full (27 GP) and Reduced (8 GP) integrations are supported]
- 2-noded discrete truss element
- 2-noded embedded truss element [At the moment, only work with 8-Noded hexahedral element]

# Supported Constitutive Models
- Von-Misses (J2-Plasticity) with elastic-perfectly plastic material behavior.
- Von-Misses (J2-Plasticity) with hardening or softening parameter.
- Rankine-Fracture plasticity model with size dependent softening function.
- Papanikolau et. al. plasticity model [2007], see [2].
- Bao et. al. plasticity model [2013], see [3].
- Piscesa et. al. plasticity model [2016] with constant and non-constant plastic dilation rate, see [4,5].
- Piscesa et. al. plasticity-Fracture model [Est. 2017] with constant and non-constant plastic dilation rate, see [6].
- Mazar et. al. damage model [2016]

# Non-Linear Solver
- Initial Stiffness Method with Process Modification.
- Initial Stiffness Method with Acceleration.
- Modifed Newton Rhapson
- Full Newton Rhapson
- Arc Length Method (Riks, Crisfield)
- Line Search
- Orthogonal Residual Method (Krenk)

# References
1. SALOME - The Open Source Integration Platform for Numerical Simulation. http://www.salome-platform.org.
2. Papanikolaou VK, Kappos AJ. Confinement-sensitive plasticity constitutive model for concrete in triaxial compression. International Journal of Solids and Structures. 2007;44:7021-48.
3. Bao J, Long X, Tan KH, Lee CK. A new generalized Drucker–Prager flow rule for concrete under compression. Engineering structures. 2013;56:2076-82.
4. Piscesa B, Attard M, Samani A, Tangaramvong S. A plasticity constitutive model for the stress-strain relationships of confined concrete. ACI Structural Journal - Accepted for publication. 2016.
5. Piscesa B, Attard MM, Samani AK. A lateral strain plasticity model for FRP confined concrete. Composite Structures. 2016;158:160-74.
6. Piscesa B, Attard MM, Samani AK. A plasticity-fracture constitutive model for concrete. Prepared to be submitted to Engineering Structures Journal.
