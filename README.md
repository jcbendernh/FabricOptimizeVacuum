# Fabric Notebooks for OPTIMIZE and VACUUM.

The purpose of this repository is to share the following notebooks so that they can be utilized to OPTIMIZE and VACUUM on a more automated fashion as opposed to manually choosing ... | Maintenance on each individual table in a Lakehouse. 

There are three notebooks in this repo, depending on your Lakehouse scenario, you'll want to select the best for your scenario:
1. If your Lakehouse does not have any schema enabled, use this notebook for OPTIMIZE and VACUUM:  [Delta Table Maintenance - No Schema - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20No%20Schema%20-%20Optimize%20and%20Vacuum.ipynb)
2. If you have Lakehouse schemas enabled and you want to run OPTIMZE and VACUUM on all schemas, use this notebook:  [Delta Table Maintenance - All Schemas - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20All%20Schemas%20-%20Optimize%20and%20Vacuum.ipynb)
3. If you have Lakehouse schemas enabled and you want to run OPTIMZE and VACUUM on only one  schema, use this notebook:  [Delta Table Maintenance - One Schema - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20One%20Schema%20-%20Optimize%20and%20Vacuum.ipynb)

**NOTE:** If you have a Lakehouse that has shortcutted tables, the OPTIMIZE and VACUUM commands may error out depending on the shortcut permissions on your source.  <br>
For example, if you only have read permissions on the source, these operations will fail.
