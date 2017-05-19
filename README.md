# Tools_BEAMnrc
Tools to create and manage BEAMnrc input files and executions

MakeNCopiesOfBEAMINP -> 

  Creates subcopies of a file. 
  Each new input has their own random number seed.
  Each new input has a unique(?) index on the end.
  For creating matching .egsinp files thAt can be excuted with simple parallelism

ChangeFileIndexString -> 

  Really just creates a string with the requested index.

ChangeRNGInFourthLineText -> 

  Changes the RNG in the text of a BEAM input file  (.egsinp).

GetFileNumberIndex -> 

  Just extracts the index for an indexed filename.
  Example: GetFileNumberIndexp["RatsNest_044,egsinp"] returns the string "044"

SetBEAMINPFileToFirstPass -> 

  Changes the restart/firstpass flag to "0" (indicating that any previous histories should be deleted.)

SetBEAMINPFileToRestart -> 

  Changes the restart/firstpass flag to "1" (indicating that any new histories should be added to an existing egsphsp file.)

CreateBEAMBatchFile -> (For Windows)
Uses the windows command "start".  Allows the user to select priority and "Wait" or "B"ackground.

SetBEAMINPNumberHistories -> 
  Changes the number of histories in the .egsinp file to the requested number.
