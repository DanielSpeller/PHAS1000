#PHAS1000 #Y1 #Thermodynamics 
We have been writing the first law as:  
$$𝑑𝑈 = 𝑑𝑄_{in} − 𝑑𝑊_{by}$$
$$𝑑𝑈 = 𝑑𝑄{in} + 𝑑𝑊_{on}  $$
For a reversible process, we have that:  
$$𝑑𝑆 = 𝑑𝑄_{rev}  $$
$$𝑇 𝑑𝑊_{on} = −𝑃𝑑𝑉  $$
And so:  
$$𝑑𝑈 = 𝑇𝑑𝑆 − 𝑃𝑑𝑉  $$
And as U, S and V are state variables, this also holds for  non-reversible processes.  
$$𝑑𝑈 = 𝑇𝑑𝑆 − 𝑃𝑑𝑉$$

However, if we have chemical reactions, then this isn’t the whole story, we are missing a term to account for the changes in the number of molecules:
$$dU=Tds-Pdv+\sum_{i}\mu_{i}dn_{i}$$
Where $𝜇_{i}$ are the chemical potentials of particles of type $𝑖$.

In fact, the system may have other parameters that change, so the general equation will be:
$$dU=Tds-Pdv+\sum_{i}\mu_{i}dn_{i}+\sum_{j}X_{j}dX_{j}$$
Where $𝑋_𝑗$ are generalized forces corresponding to the parameters $𝑥_𝑗$

- Intensity variable: the magnitude does not depend on the amount of substance in a closed system.  
- Extensive variable: the magnitude depends on the amount of substance present in a closed system.

For example, if I have a problem where electric charges are being moved, then my first law relation will have an additional term:
$$dU=Tds-Pdv+\sum_{i}\mu_{i}dn_{i}+vdQ$$
In mechanics, the gravitational potential is an arrow that shows in which direction masses tend to move: from a high  
towards a low potential. The same way we can define a chemical potential that will indicate in which direction a chemical composition will tend to evolve.

From the fundamental thermodynamic relation, we can derive a definition of the chemical potential by using the [[Partial Differentiation|partial derivative]].
$$dU=Tds-Pdv+\sum_{i}\mu_{i}dn_{i}$$
$$\mu_{i}=\left(\frac{\partial U}{\partial n_{i}}\right)_{S,V,n_{j\neq i}}$$
That is, if we keep $𝑆$, $𝑉$ and all other species constant, the chemical potential $𝜇_{i}$ is the change of internal energy when  
we change the number of molecules of species $𝑖$

For systems in equilibrium, we will see that as we change the temperature, the system will minimize the chemical potential.

Alternatively, we will introduce a different thermodynamics potential: Gibbs free energy, which is defined for constant pressure
$$\mu_{i}=\left(\frac{\partial G}{\partial n_{i}}\right)_{S,P,n_{j\neq i}}$$
Enthalpy is a state function that depends on $𝑇, 𝑃, 𝑈$:  $𝐻 ≡ 𝐻(𝑇, 𝑃, 𝑈)$  
When a process occurs at constant pressure, the heat exchanged is equal to the change of enthalpy $Δ𝐻$.  
$𝐻 = 𝑈 + 𝑃𝑉$

If we differentiate this
$$dH=DU+PdV+VdP=TdS+VdP$$
$$dH=Q_{rev}=TdS$$
Enthalpy of phase transitions are often standard molar quantities (Δ𝐻0)  
- Standard enthalpy of vaporization $𝚫𝑯_{𝒗𝒂𝒑}^0$ : energy that must be supplied as heat at constant pressure per mole of molecules  vaporized (liquid to gas).  
- Standard enthalpy of fusion $𝚫𝑯_{fusion}^𝟎$ : energy that must be supplied as heat at constant pressure per mole of molecules melted (solid to liquid).  
- Standard enthalpy of sublimation $𝚫𝑯_{𝒔𝒖𝒃}^𝟎$ : energy that must be  supplied as heat at constant pressure per mole of molecules  sublimated (solid to gas).


Gibbs free energy can predict the direction of a chemical reaction under constant pressure and temperature, and  is a state function.:
$$G=U+PV-TS$$
$$G=H+TS$$
1. If the “available energy” in a system for a particular process is increasing, then it will need to come from somewhere: this will only happen if there is an external input (non-spontaneous):  $Δ𝐺 > 0$
2. If the “available energy” in a system for a particular process is decreasing, then the system should have enough energy to run the process (spontaneous): $Δ𝐺 < 0$


Helmholtz free energy is a state function we define as:
$$F=U-TS$$
$$dF=dU-TdS-SdT$$
If we substitute the first law (without changes in chemical composition)
$$dF=TdS-PdV-TdS-SdT$$
$$dF=-PdV-SdT$$
Helmholtz free energy measures the useful work obtainable from a closed thermodynamic system at a constant  
temperature and useful if we cannot have a constant pressure.

From the definition of Gibbs energy we learned:  
$$𝐺 = 𝐻 − 𝑇S = 𝑈 + 𝑃V − 𝑇S$$

When differentiating a product, we always get two terms:  
$$𝑑𝐺 = 𝑑𝑈 + 𝑃𝑑𝑃V + V𝑑𝑃 − 𝑇𝑑S −S𝑑𝑇  $$
Now we can use the definition of $𝑑𝑈$:  
$$𝑑𝐺 = 𝑇𝑑S − 𝑃𝑑𝑃V + 𝜇 _𝑖 𝑑𝑛 _𝑖 + 𝑃𝑑V + V𝑑𝑃 − 𝑇dS − Sd𝑇  $$
$$𝑑𝐺 = Vd𝑃 − S𝑑𝑇 +𝜇_𝑖 𝑑𝑛_𝑖$$
For each thermodynamic potential, there are a set of variables that need to be held constant to specify the value of the potential at equilibrium, known as the natural variables.  
- T and S are never natural variables together  
- V and P are never natural variables together

From the Clausius inequality, we learned that for a cycle:
$$\oint\frac{\delta Q}{T}\geq 0$$
If our cycle is reversible, then
$$\delta Q \equiv \delta Q_{rev}$$
$$\oint \frac{\delta Q_{rev}}{T}=S_{cycle}=0$$
If our cycle is irreversible, then
$$\oint \frac{\delta Q_{irrev}}{T}<0$$
$$\oint \frac{\delta Q_{irrev}}{T}< \frac{\delta Q_{rev}}{T}=S_{cycle}$$
$$\delta Q_{rev}>\delta Q_{irrev}$$
$$dS\geq \frac{\delta Q}{T}$$
$$dU=\delta Q_{in}+dW_{on} \leq TdS+dW_{on}$$
$$dU\leq TdS-PdV+\sum_{i}\mu_{i}dn_{i}$$
At constants $S$, $V$ and $n_i$ we have that 
$$du\leq 0 \rightarrow \text{equilibrium} \ dU=0 \ , \text{spontaneous} \ dU<0$$
$$H=U+PV$$
$$dH=\left( \delta Q_{in}-PdV+\sum_{i}\mu_{i}dn_{i} \right)+pdV+VdP\leq TdS+VdP+\sum_{i}\mu_{i}dn_{i}$$
For a process at constant $𝑇$, $𝑃$ and $𝑛_i$, we have that
$$dH\leq 0 \rightarrow \text{equilibrium} \ dH=0 \ , \text{spontaneous} \ dH<0$$
$$F=U-TS$$
$$dF=\left( \delta Q_{in}-PdV+\sum_{i}\mu_{i} dn_{i} \right)-TdS-SdT\leq TdS-PdV-TdS-SdT+\sum_{i}\mu dn_{i}$$
$$dF\leq-PdV-SdT+\sum_{i}\mu_{i}dn_{i}$$
For a process at constant $V$, $T$ and $𝑛_i$, we have that
$$dF\leq 0 \rightarrow \text{equilibrium} \ dF=0 \ ,  \ \text{spontaneous} \ dF<0$$
This has its use specially for systems where $dn$ changes for different species.
$$G=U+PV-TS$$
$$dG=\left(Q_{in}-PdV+\sum_{i}\mu_{i}dn_{i}\right)+PdV+VdP-TdS-SdT\leq\left( TdS-PdV+\sum_{i}\mu_{i}dn_{i} \right)+PdV+VdP-TdS-SdT$$
$$dG\leq VdP-SdT+\sum_{i}\mu_{i}dn_{i}$$
At constant $P$, $T$ and $n_i$ we have that
$$dG\leq 0\rightarrow \text{equilibrium} \ dG=0 \ , \ \text{spotaneous} \ dG>0$$
Gibbs Helmholtz equation
$$G=H-TS$$
$$dG=dH-SdT-TdS$$
Isothermally
$$dG=dH-TdS$$
$$\Delta G=\Delta H-T\Delta S$$
For constant pressure
$$dG=VdP-SdT+\sum_{i}\mu_{i}n_{i}$$
$$d\left( \frac{G}{T} \right)=\frac{1}{T}dG+\left( -\frac{1}{T^2} dT\right)G=\frac{TdG-GdT}{T^2}$$
$$d\left( \frac{G}{T} \right)=\frac{T(VdP-SdT)-GdT}{T^2}=\frac{TVdP-(TS+G)dT}{T^2}=\frac{TVdP-HdT}{T^2}$$
$$\left(\frac{\partial\left( \frac{G}{T} \right)}{\partial T}\right)_{P}=\frac{-H}{T^2}$$
Maxwells relations
$$dG=-SdT+VdP$$
$$\left( \frac{\partial G}{\partial T} \right)_{P}=-S$$
$$\left( \frac{\partial G}{\partial P} \right)_{T}=V$$
$$\left( \frac{\partial}{\partial P}\left( \frac{\partial G}{\partial P} \right) \right)_{T}=-\left( \frac{\partial S}{\partial P} \right)_{T}$$
$$\left( \frac{\partial}{\partial T}\left( \frac{\partial G}{\partial P} \right) \right)_{P}=\left( \frac{\partial V}{\partial T} \right)_{P}$$
Due to the [[Partial Differentiation|symmetry of second derivatives]] the same result is yielded
$$-\left( \frac{\partial S}{\partial P} \right)_{T}=\left( \frac{\partial V}{\partial T} \right)_{P}$$
