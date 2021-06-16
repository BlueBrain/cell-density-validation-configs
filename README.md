This repository contains configuration files to be used together with:
git@bbpgitlab.epfl.ch:conn/structural/validation/cell-density-validations.git

Note: The paths in the files in this master branch are need to be adapted to the specific circuit used.
Paths under the "annotations" and "hierarchy" keys need to be updated to point to the atlas to be used; paths under "nrrd" need to be updated to point to the files to be validated. The path under "circuits" needs to be updated to point to the circuit to be validated.
Paths in the branches of the repository have been updated thus for the validation of specific releases.

The validations are to be run at the following steps of the cell-density-building pipeline:
1) After the first step that generates EXC, VIP, SST, PV and REST densities (Dimitri), run a validation against consistency_checks_density_inputs.json
2) After the generation of densities for inhibitory m-types (Yann), run a validation against consistency_checks_inh_density_outputs.json
3) After the generation of excitatory densities, run a validation against consistency_checks_exc_density_outputs.json
4) After a circuit has been built, validate it using circuit_test_all_densities.json

