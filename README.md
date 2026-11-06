# Dynamic CDS creation based on table name as input
DATA(lr_instance) = NEW zcl_cds_maint_dynamic( iv_tablename ).
lr_instance->generate_cds_view( ).
MOVE lr_instance->m_cds TO rs_cds.

