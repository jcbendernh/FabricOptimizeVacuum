# Fabric Notebooks for OPTIMIZE and VACUUM commands

This repository provides a set of PySpark notebooks designed to help Microsoft Fabric Data Engineers automate the execution of OPTIMIZE and VACUUM operations across all Lakehouse tables—without the need to manually select each table through the GUI

There are three notebooks in this repository—select the one that aligns best with your specific Lakehouse scenario:
1. If your Lakehouse does not have any schema enabled, use this notebook for OPTIMIZE and VACUUM:  [Delta Table Maintenance - No Schema - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20No%20Schema%20-%20Optimize%20and%20Vacuum.ipynb)
2. If you have Lakehouse schemas enabled and you want to run OPTIMZE and VACUUM on all tables in all schemas, use this notebook:  [Delta Table Maintenance - All Schemas - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20All%20Schemas%20-%20Optimize%20and%20Vacuum.ipynb)
3. If you have Lakehouse schemas enabled and you want to run OPTIMZE and VACUUM on all tables in only one  schema, use this notebook:  [Delta Table Maintenance - One Schema - Optimize and Vacuum](notebooks/Delta%20Table%20Maintenance%20-%20One%20Schema%20-%20Optimize%20and%20Vacuum.ipynb)

**NOTE:** If you have a Lakehouse that has shortcutted tables, the OPTIMIZE and VACUUM commands may error out depending on the shortcut permissions to your source.  <br>
For example, if you only have read permissions on the source, these operations will fail for that specific table.

These are the progression of a notebook shared by [Luke Newport](https://www.linkedin.com/in/lukenewport/) and thanks to [Zach Christoff](https://www.linkedin.com/in/zach-christoff-485b7466/) for his input as well.
