# Identifying_Entities_in_Healthcare_Data

## Data Preprocessing

The dataset provided is in the form of one word per line. Let's understand the format of the data below:
- Suppose there are *x* words in a sentence, then there will be *x* continuous lines with one word in each line. 
- Further, the two sentences are separated by empty lines. The labels for the data follow the same format.

**We need to pre-process the data to recover the complete sentences and their labels.**


"BeHealthy" is a health-tech company that operates a web platform enabling doctors to list their services and manage patient interactions. The platform offers various services for patients, including booking interactions with doctors and ordering medicines online. Within this platform, doctors can efficiently organize appointments, track past medical records, and provide e-prescriptions. Consequently, companies like "BeHealthy" are facilitating medical services, prescriptions, and online consultations, resulting in the accumulation of substantial data over time.

Within the medical data generated, we encounter snippets like the following example: "The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy."

This excerpt illustrates the challenge faced by individuals without a medical background in understanding various medical terms. It provides a simplified instance from a medical dataset, wherein terms like 'cancer' and 'chemotherapy' might be comprehensible to non-medical individuals.

We possess a dataset comprising extensive text related to the medical domain. Across the dataset, numerous diseases and their corresponding treatments are mentioned implicitly. In the example provided, the disease highlighted is cancer, with its treatment indicated as chemotherapy. Although not explicitly stated, we can develop an algorithm to establish associations between diseases and their respective treatments.

The training dataset is utilized to train the Continuous Random Field (CRF) model, while the test dataset serves to evaluate the constructed model.
