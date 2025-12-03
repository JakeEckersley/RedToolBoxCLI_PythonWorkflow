# RedToolBoxCLI_PythonWorkflow
This workflow applies PPK corrections to the coordinates contained in the EXIF files of drone imagery (mavic M3E MS). It uses python (jupyter) to communicate with the RedCatch RedToolbox command line interface allowing the workflow to be batch processed. The script works off a spreadsheet containing paths of drone flights, a DGPS base station (reach RS2), their associated metadata, and outputs from base station PPK corrections (AusPos).

The resulting outputs are ready to be passed to metashape which is accessed via the python API and batch processed using the initial metadata spreadsheet.
