# Media and Metadata to Text Generation 

## Overview
This repository provides a series of Jupyter notebooks designed to convert media and its associated metadata into informative text. This process is beneficial for tasks such as automated content creation, summarization, and enhanced metadata tagging. The workflow includes generating captions for images and text, extracting textual content from media, combining this information with additional metadata, and finally generating comprehensive text using a language model.

### Workflow:
1. **Caption Generation**: Generate captions for images using the `Blip2-caption-generation.ipynb` notebook.
2. **Text Extraction**: Extract text from media using OCR with the `Text-extraction-from-media-by-ocr.ipynb` notebook.
3. **Instruction Data Creation**: Combine captions, extracted text, and metadata into a single prompt using the `Making-instruction-data-for-task2.ipynb` notebook.
4. **Text Generation**: Generate the final text output based on the combined prompt using the `Inference_Llama2.ipynb` notebook.

## Notebooks Description

### 1. Blip2 Caption Generation (`Blip2-caption-generation.ipynb`)
- **Purpose**: Generates captions for images and text within the media.
- **Outputs**: Descriptive captions for each image or piece of media.

### 2. Text Extraction from Media by OCR (`Text-extraction-from-media-by-ocr.ipynb`)
- **Purpose**: Extracts any textual content present in the image or thumbnail using Optical Character Recognition (OCR) technology.
- **Outputs**: Text extracted from the media.

### 3. Making Instruction Data for Task 2 (`Making-instruction-data-for-task2.ipynb`)
- **Purpose**: Combines the generated captions, extracted text, and additional metadata (such as author, date, etc.) into a single structured prompt.
- **Outputs**: A comprehensive prompt that encapsulates all relevant information from the media and its metadata.

### 4. Inference with Llama2 (`Inference_Llama2.ipynb`)
- **Purpose**: Generates the final text output based on the combined prompt using the Llama2 language model.
- **Outputs**: Final generated text that reflects the content and context of the original media and its metadata.
