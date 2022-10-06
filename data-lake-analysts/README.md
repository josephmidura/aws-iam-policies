I have one AWS managed policy, AmazonAthenaFullAccess, and two inline policies that should be applied to IAM users in the data-lake-analysts group:

allow-athena-bucket-access.json
datalakeUserBasic.json

10/6/22
The WCWH group doesn't need AmazonAthenaFullAccess, and instead needs this more restricted policy:

Athena-primary-workgroup-run-queries.json