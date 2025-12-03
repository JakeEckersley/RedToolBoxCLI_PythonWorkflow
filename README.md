# RedToolBoxCLI_Metashape_PythonWorkflow
This workflow applies PPK corrections to the coordinates contained in the EXIF files of drone imagery (mavic M3E MS) then stitches together the imagery using metashape. The final export is PPK corrected rgb orthomosaic, spectrally calibrated reflectance data, a DEM and surface elevation model. It uses python (jupyter) to communicate with the RedCatch RedToolbox command line interface and Metashape via the python API allowing the workflow to be batch processed. 

The scripts work off an excel spreadsheet containing paths to raw imagery from drone flights (and their associated metadata), the paths to DGPS base station outputs (reach RS2 rinex files), and outputs from base station PPK corrections (AusPos). An example of the spreadsheet formatting is attached.

We had problems with both metashape and redcatch connecting to our remote data repository so the script also contains code to create a temporary local folder for all processing and returns the outputs to the online repository once everything is processed.
