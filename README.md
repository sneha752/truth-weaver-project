Truth Weaver: AI-Powered Transcript Analysis
Overview
Truth Weaver is a Python script designed to analyze text transcripts, identify key information, and detect potential deception patterns. By integrating the Gemini API, the script can provide a sophisticated, context-aware analysis of human communication, offering insights into programming experience, skill mastery, leadership claims, and more.

How It Works
The script performs the following actions:

Reads Transcripts: It scans a specified directory for all files ending with _transcript.txt.

Analyzes with AI: Each transcript is sent to the Gemini API with a detailed prompt and a specific JSON schema.

Generates Structured Output: The AI's response is a JSON object containing a "revealed truth" summary and a list of "deception patterns" found in the text.

Saves Results: The analysis for each transcript is saved as an individual .json file, and a combined JSON file is created for all transcripts in the directory.

Getting Started
Prerequisites
Python 3.6+

The requests library (pip install requests)

Access to the Gemini API (the API key is handled by the Canvas environment)

Usage
Place your transcript files (e.g., interview1_transcript.txt) in the src directory.

Run the script from your terminal:

python truth_weaver_gemini.py

The script will output .json files for each transcript and a combined all_transcripts_output.json file in the same directory.