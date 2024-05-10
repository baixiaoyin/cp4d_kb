# This is the repo for the instructlab training

- answer: Install Cloud Pak for Data platform operator and service operator of watsonx_data.
    cpd-cli manage apply-olm release=${VERSION} cpd_operator_ns=${PROJECT_CPD_INST_OPERATORS} components=watsonx_data
    Install the operands in the operands project for the instance of watsonx_data.
    cpd-cli manage apply-cr \
    --release=${VERSION} \
    --cpd_instance_ns=${PROJECT_CPD_INST_OPERANDS} \
    --components=watsonx_data \
    --block_storage_class=${STG_CLASS_BLOCK} \
    --file_storage_class=${STG_CLASS_FILE} \
    --license_acceptance=true
  question: What are the commands to install watsonx_data?
- answer: Install Cloud Pak for Data platform operator and service operator of watsonx_ai.
    cpd-cli manage apply-olm release=${VERSION} cpd_operator_ns=${PROJECT_CPD_INST_OPERATORS} components=watsonx_data
    Install the operands in the operands project for the instance of watsonx_data.
    cpd-cli manage apply-cr \
    --release=${VERSION} \
    --cpd_instance_ns=${PROJECT_CPD_INST_OPERANDS} \
    --components=watsonx_data \
    --block_storage_class=${STG_CLASS_BLOCK} \
    --file_storage_class=${STG_CLASS_FILE} \
    --license_acceptance=true
  question: What are the commands to install watsonx_ai?
