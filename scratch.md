

```sh

export COPYBOOK=/u/CARMIS1/mfc/copybooks/test_data.cpy
export LOG_PROJECT=<project Id>
export LOG_ID=<log Id>
export OUTFILE=<output file>
export OUTFILE_LRECL=<lrecl size>

bq export --project_id=atomic-rune-427309-e8       \
    --dataset_id="export_test"                     \
    --destination_table=test-188M --location="US"  \
    --timeOutMinutes=200000                        \
    --sql="select * from test-188M"

```
