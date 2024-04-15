> **COMP-841 Practical AI**
# Fine-tuning a Pretrained LLM

#### Purpose
- Learn about Fine-tuning large language model(LLM) for natural language processing (NLP) tasks.
- Become familiar with fine-tuning pre-trained language models for specific natural language processing (NLP) tasks, such as question answering, sequence classification, using the Hugging Face Transformers library.


#### Getting Started

1. **Get the codebase:**
   - Sign into your SageMaker Studio Lab account and select GPU as the compute type, then start the runtime and open the project.
   - Open a terminal and change the directory to the home directory.
   - Change directory to the home directory.
   - If not already present, create a folder named `comp841` or `comp741`.
   - Navigate to the root directory of the course.
   - Clone the lab repository (lab_number) using the GitHub Classroom invitation link (see Discord).
   ```
   git clone <URL of lab_number> lab_number
   ```

2. **Setup and Environment:**

   - The HuggingFace Transformers library caches downloaded models. Create a separate .cache directory in the lab root directory to avoid space issues.
      - In a terminal within the lab_number directory, Confirm the directory by running `pwd`
      - `mkdir .cache` to create the `.cache` directory
   - To avoid running out of space, delete old unused environments:
      - List environments: 
      ```
      conda env list
      ```
      - Remove old environments:
      ```
      conda remove -n ENV_NAME --all
      ```
   - Create the lab_number virtual environment from the `fine_tune_env.yml` file:
   ```
   conda env create -n fine_tune_env --file=fine_tune_env.yml
   ```

#### Requirements

- Read, run, and experiment with the `fine_tuning_llm.ipynb` notebook in the lab_number directory.
- Create an `EXPERIMENT.md` file to log information about additional experimentation with the fine-tuning process demonstrated in the notebook.
- In the `EXPERIMENT.md` file, include two sections with heading level three (e.g., `### Observations`): one for recording experimental information and another for answering questions.
- Version control the completion of this activity by committing changes made to the `EXPERIMENT.md` file.

### Submission:

#### GitHub:
- Push the commit history of writing the files to your GitHub repository.

#### Canvas:
- Convert the `EXPERIMENT.md` file to PDF format and Upload it to the Canvas submission link.
