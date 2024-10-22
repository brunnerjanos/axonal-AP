brunner 2024 at KOKI
............................................

Each file in the root directory contains simulations and parameter optimizations associated with individual axonal recordings (with the filename corresponding to the recording identifier).

Each experimental file includes the following folders:

'Rrest_Cm_in_situ_discretized'
'AP_fits_bjd####_1_long_window_eK=-90mV_discretized'



Conceptual Overview of the Simulations:
The model reconstitution of the actual experiment involves two optimization steps:

1- Rrest_Cm_in_situ_discretized;
In the first step, we adjusted the passive electrical properties of the model axon . This included tuning parameters such as membrane capacitance (Cm), axial resistance (Ra), access resistance (Raccess), and pipette capacitance (Cpip) to match the experimentally measured subthreshold signals.
Necessary Experimental Inputs:
	Filter settings used in the experiment
	Bridge-balance compensation settings
	Applied capacitance neutralization
Seal Resistance:
	The seal resistance (Rseal) was calculated based on the measured resting membrane potential. For theoretical details, see Oláh, Tarcsay, and Brunner (2011).

Realistic Morphology:
	The axon's morphology was reconstructed in detail, covering approximately 140 µm around the recording site. This reconstructed portion was extended with idealized dummy compartments, typically on both sides, to complete the model.

Rm was held constant (50 kΩ*cm2)


2- AP_fits_bjd####_1_long_window_eK=-90mV_discretized;
In this step, we fine-tuned the parameters of the active sodium and potassium current models to accurately reproduce the experimentally measured action potential shape.
Necessary Inputs:
	Realistic Morphology
	Passive parameters and pipette capacitance that were optimized in the first step.
	Experimentally used settings
	Seal resistance 
The model output provides the optimal parameter set for the ion channel models, enabling a faithful recreation of the recorded APs.
With these optimizations, we can predict both the shape and magnitude of the underlying ionic currents, as well as the native AP morphology.


sMF experiments are:
bjd1196_2
bjd1202
bjd1203_3
bjd1209
bjd1253
bjd1311_1
bjd1312_1
bjd1346_sl2_3
bjd1375_2
bjd1378_1
bjd1381_1
bjd1384_1
bjd1385_1
bjd1412_2
bjd1418_1
bjd1421_2
bjd1438_2
bjd1442_6

LMFB experiments are:
bjd1204_1
bjd1205_1
bjd1206
bjd1252_3
bjd1373_2
bjd1374_1
bjd1383_2
bjd1403_1
bjd1404_3
bjd1438_1
bjd1439_3

