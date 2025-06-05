All the files are ipynb files, which can be easily run directly. All you need to do is change the path according to the main folder. All the work has been categorised into sections/subsections for ease of access.
I have done most of the work in colab. This is the drive link: https://drive.google.com/drive/folders/1215z9FrydK8Qn9wM2u3e8l427S1mzvw4?usp=sharing

The codebase folder contains all the ipynb files-
The main files are gemini.ipynb and openai.ipynb
They both contain the prompts I ran for all the steps(baselines and neurosymbolic)
Direct and CoT prompting
Few shot
API extraction
Neurosymbolic generation

There are two other ipynb files for auto eval using gemini and openai titled: gemini_rule_based_checking and openai_rule_based_checking

api_doc_extraction.ipynb extracts documentation for the selected APIs/libraries list

few_shot_prompt_creation creates the prompt for the few shot baseline

The Dataset folder contains the list of tasks finally decided and the few shot examples that have also been selected manually. Initially the data and datagen folders were created to look at the type of data that could be scraped and used, but eventually the tasks were manually picked and aligned due to lack of diversity.

The CSV folder contains all the essential csv files:
Prompts-step2:  prompts.csv : Contains direct and cot prompts
Few_shot_prompts.csv: Few shot prompts
Api_documentation_new.csv: Api documentation followed by responses of gpt and gemini’s extracted version
Neural_results_gpt.csv: Neural suggestion results gpt
Neural_results_gemini.csv: Neural suggestion results gemini
Symbolic_gpt.csv: Symbolic checking suggestion gpt(Rules to be looked into)
Symbolic_gemini.csv: Symbolic checking suggestion gemini(Rules to be looked into)
Check_gemini.csv: Output for GPT after symbolic checking
Check_gpt.csv: Output for Gemini after symbolic checking
Final_generated_code_gemini.csv: Final generated code gemini
Final_generated_code_gpt.csv: Final generated code gpt
Step2-responses.csv: Responses all put together for step2 (Responses of baselines like direct, cot, few shot and neurosymbolic synthesis)


The evaluation folder contains a code folder and some excel sheets for evaluation and score compilation. 
Code: Runtime files for all the cases : GPT+Gemini(Few shot,CoT,Direct) = 2*3 = 6
					  GPT+Gemini (Neurosymbolic) = 2
	Code_quality: To check quality of code
	Compilation_success_rate:  To check compilation and syntax quality
	Extract_code_snippets: To extract code from the response

code_quality&runtime_check: Final compiled values for code quality and runtime check
Generalization: generalization test cases
Eval: contains evaluation details
Final_code_gpt: final clean code for gpt
Final_code_gpt.csv: final clean code for gpt
Final_code_gemini.csv: final clean code for gemini

The excel and google sheets folder contains the excel version of csv. Details remain the same.
	
