### Instructions for creating the Comparison with Argonaut Data Query IG folder

1. Use the [FHIR validator]() to compare and the script /Users/ehaas/Documents/Python/Jupyter/MyNotebooks/Validator_Tools/IG-Profile_Comparer.ipynb with the source file input/images-source/ArgoDQ-USCore-ProfileMap.csv.
1. See the script file for instructions
2. Note that only the comparison files are used the union and intersection files are discarded.
3. for ig publisher >>>>>>  Need to clean up the generated html files to remove the QA errors
   1. look for "null" and remove  ( e.g. in /Users/ehaas/Documents/Python/Jupyter/MyNotebooks/utils/out/profile_compare/temp_out/sd-argo-goal-us-core-goal.html)
      1. find ` null"` and replace with `"`
   2. fix bad links for publisher using regex
      1. find '<a href="\?\?.*?>(.*?)</a>'
      2. replace '$1'
