#What was done in the week 
Identified what actually worked vs what was skeleton code
TORCS-Jamie had the most complete race engineer — kept that as the base
Started writing README.md with setup and deployment instructions
Created unified requirements.txt across all branches

##Key decisions

All AI features to use Ollama granite4:3b
MockTORCSClient for testing without TORCS running
Single command to run each feature from project root

##Challenges

test_ollama.py had wrong model name (granite3.3:2b instead of granite4:3b)
torcs_jm_par.py had unresolved merge conflict markers

##Fixed by

Updated model name in test file
Resolved merge conflicts, kept the more complete version

'requirements.txt' - 
ollama
pyttsx3
Pillow
transformers
torch