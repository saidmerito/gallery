# Turning Handwritten Medical Registers into Usable Data

This project demonstrates an offline mobile workflow using Gemma in AI Edge Gallery to extract handwritten medical register data from images and convert it into structured CSV format.

## Workflow

1. Open AI Edge Gallery on Android.
2. Select the Gemma model.
3. Use Ask Image to import a handwritten medical register photo.
4. Ask Gemma to extract the visible information.
5. Convert the extracted data into CSV format.
6. Copy and save the CSV output for later review and use.

## Extraction Prompt

```text
You are a health data extraction assistant.

Analyze this image of a handwritten medical register and extract the visible information into a clean CSV table.

Use the following columns:
Date, Patient_ID, Patient_Name, Age, Sex, Diagnosis, Treatment, Remarks

Rules:
- Return only CSV format.
- Use one row per patient or register entry.
- Keep the original meaning of the handwritten text.
- If a value is missing, write EMPTY.
- If a value is unclear or difficult to read, write UNCLEAR.
- Do not invent information.
- Do not add explanations before or after the CSV.
