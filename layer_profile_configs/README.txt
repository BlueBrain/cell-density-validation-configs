These configuration files are to be used in conjunction with https://bbpgitlab.epfl.ch/conn/structural/validation/cell-density-validations/-/blob/master/cell-densities/bin/extract_depth_profiles.py

These specific configuration files came along because we had to update the code generating the excitatory cell densities. 
The change was required in order to fulfill the consistency tests. We wanted to assure that this intervention did not completely destroy the biological validity of the profiles.

Therefore, these two configs extract profiles before (pre) and after (post) the intervention. For later comparison

In terms of reproducibility, we are going to overwrite the (pre) files in the atlas directory with the (post) files after validation.
Therefore, you won't be able to reproduce the result with the paths given in these configs. Sorry about that.

Regardless, we will add the result files also to this repository. They are the result of executing the script linked above with these configuration files at 11.06.2021.

  --MWR
