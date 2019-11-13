armi-plugin-directory
=====================
A list of known ARMI plugins for use with https://github.com/terrapower/armi.

Note: Many of the codes referred to on this page are copyrighted by their
respective institution.

TerraPower open source plugins
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The following plugins are available on this project's GitHub page.

.. list-table:: 
   :widths: 25 50 25
   :header-rows: 1

   * - Plugin name
     - Description
     - Comments
   * - `DRAGON ARMI plugin <https://github.com/terrapower/dragon-armi-plugin>`_
     - Run École Polytechnique de Montréal's DRAGON code
     - Makes ISOTXS formatted library; allows template customization for more advanced usage.


Community plugins
^^^^^^^^^^^^^^^^^
.. list-table:: 
   :widths: 25 50 25
   :header-rows: 1

   * - Plugin name
     - Description
     - Comments
   * - Your Plugin here
     - Description
     - Comments

TerraPower commercial plugins
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The following plugins exist and may be available with commercial licensing. 
Contact armi-devs@terrapower.com for more info. 

.. list-table:: 
   :widths: 25 50 25
   :header-rows: 1

   * - Plugin name
     - Description
     - Comments
   * - Windows HPC plugin
     - Submit jobs and tests to a Windows HPC environment
     - 
   * - Crucible
     - A fast-running metallic fuel performance code
     - Driven off of longer-running ALCHEMY runs
   * - Depletion
     - Solves nuclear transmutation and decay problems in parallel 
     - CRAM and Pade methods
   * - TP's DIF3D plugin
     - Write input files for ANL's DIF3D code, run DIF3D, read DIF3D output state
     - Hex, RZ, RZTheta, and Cartesian geometry
   * - Economics
     - Computes levelized cost of electricity for an ARMI scenario 
     - Largely focused on fuel cycle costs (SWUs, feed, fab, etc.)
   * - Equilibrium fuel cycle
     - Computes the implicit equilibrium fuel cycle quickly
     - Similar to ANL's REBUS-3 code
   * - Fluxrecon
     - Computes continuous inter-assembly flux and power distributions
     - Essential for subchannel T/H analysis
   * - Gamma transport
     - Updates power distribution considering the explicit transport of photons. 
     - Important for sophisticated T/H calcs
   * - Intrinsic source
     - Computes spontaneous fission source throughout ARMI scenario
     - Useful for startup detector signal analysis
   * - TP's MC2 plugin
     - Write input files for ANL's MC**2-3 code, run MC2, read output state
     - Good for generating fast reactor cross sections
   * - TP's MCNP plugin
     - Write input files for LANL's MCNP code, run MCNP, read output state
     - Pin detailed or homogenized
   * - TP's NJOY plugin
     - Can drive LANL's NJOY code for a variety of nuclear data uncertainty purposes
     - Like covariance data
   * - Nuclear Data UQ
     - Computes sensitivities of a core to each cross section using generalized
       perturbation theory. Loads covariance data from NJOY and evaluates the
       sandwich formula to determine the uncertainty in integral nuclear
       performance metrics due to nuclear data uncertainty.
     - Handles keff and reactivity coefficients so far. Power distribution planned.
   * - TP's PARTISN plugin
     - Runs LANL's PARTISN code either as a global flux solver or as a
       simplified high energy resolution solver in a 2-step process for
       generating cross sections with MC2 in non-fissile regions (like
       reflectors)
     - 
   * - Reactivity control
     - Moves control rods up and down, performs criticality searches, finds
       highest-worth rods (in parallel), etc.
     - Depends on external physics solvers to compute keff
   * - TP's REBUS plugin
     - Drives several features of ANL's REBUS fuel cycle code
     - Largely superseded by Equlibrium plugin
   * - Reactivity coefficients
     - Computes kinetics parameters (like beta-effective), core-wide reactivity
       coefficients, and spatially-dependent reactivity coefficients in
       arbitrary sections of a core. 
     - Essential input for transient analysis
   * - TP's SASSYS plugin
     - Writes the core elements to input files for ANL's SASSYS code, including
       power and flow distribution, reactivity coefficient distributions,
       composition. Combines with a user-provided plant model to perform
       transient analysis.  
     - Can also perform statistical sweeps to compute
       sensitivity of peak clad temperature (or other metrics) to various
       inputs
   * - TP's Serpent plugin
     - Writes VTT's Serpent inputs for cross section generation
     - Mostly targeting SFR assemblies
   * - Source term
     - Computes the source term
     - Important for safety analysis
   * - Stability
     - Computes the zero power transfer function and the full power transfer
       function of a core using a plant transient model (e.g. SASSYS) running a
       frequency sweep of programmed oscillatory reactivity. The performs
       signal processing analysis to determine the phase and gain margins of
       stability for a plant.  
     - Important
   * - SFR Thermal/Hydraulics
     - Performs subchannel T/H analysis with a variety of TerraPower physics
       kernels including *subchan* and *MONGOOSE*. Also computes flow orificing
       required for a given x-year fuel management scenario without
       undercooling.  
     - SFR/single-phase focused
   * - VirDenT
     - Computes the reactivity feedback resulting from arbitrary 3D core
       mechanical perturbations. Essential for radial expansion and core
       restraint study.  
     - Couples closely with subchannel T/H, core
       mechanical, and fluxRecon modules



