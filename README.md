Resume VLM Screener – AI That Sees Hidden Prompts

Defeats AI resume bypass tricks** by converting PDF → Image → Vision LLM (Gemini)

"Hidden prompt" in resume? Not anymore.


 How to Use

 1. Import Workflow
→ Click [resume-vlm-screener.json](resume-vlm-screener.json) → Copy all  
→ In n8n: New → Import from Clipboard (or drag file)

 2. Fix Red Warnings (Credentials)
Create these exact names:

| Credential | Name |
|----------|------|
| Google Drive | `Google Drive account` |
| Google Gemini (PaLM) | `Google Gemini(PaLM) Api account` |

 3. Setup
- Resume PDF ID: Already set to test file  
  [Download test resume with hidden prompt](https://drive.google.com/file/d/1MORAdeev6cMcTJBV2EYALAwll8gCDRav/view?usp=sharing)
- Stirling PDF API: Uses public `stirlingpdf.io` (for demo only)

 4. Test
1. Click "Test workflow"
2. Wait → Output:
   ```json
   { "is_qualified": false, "reason": "Hidden prompt detected..." }
