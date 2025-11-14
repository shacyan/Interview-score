# Interview Scoring System

A comprehensive web-based interview scoring system designed for conducting technical interviews with multiple candidates. Built specifically for Infrastructure Support Engineer (SRE) positions but can be customized for any role.

## Features

- **Individual Interview Mode**: Interview candidates one-by-one with full tracking
- **Progress Tracking**: Visual progress bars and completion badges for each candidate
- **Comprehensive Scoring**: 0-10 scale scoring with detailed notes for each answer
- **Multiple Sections**: Organized by skill areas with customizable weights
- **Summary Dashboard**: Automatic ranking, percentage calculations, and detailed breakdowns
- **Export Options**: Export results to JSON or CSV formats
- **Import Capability**: Load questions from JSON or CSV files
- **Sample Questions**: Pre-loaded with 25 SRE interview questions

## Quick Start

### Option 1: Use Pre-loaded Sample Questions

1. Open `index.html` in your web browser
2. Click **"Load SRE Sample"** button
3. Enter candidate names (comma-separated): `Pramod, Eshani, Chaveen, Ishara`
4. Click **"Set Candidates & Start"**
5. Select a candidate and begin scoring their answers
6. Navigate through questions using Previous/Next buttons
7. Click **"Finish Candidate"** when complete
8. View summary and export results

### Option 2: Load Questions from File

**Using JSON:**
1. Click **"Load Questions (JSON)"**
2. Select `sre-interview-questions.json`
3. Follow steps 3-8 from Option 1

**Using CSV:**
1. Click **"Load from CSV"**
2. Select `sre-interview-questions.csv`
3. Follow steps 3-8 from Option 1

## Interview Sections

The SRE interview includes 9 sections with weighted scoring:

| Section | Weight | Questions | Max Score |
|---------|--------|-----------|-----------|
| Monitoring & Observability | 25% | 4 | 40 |
| AWS Technical Knowledge | 20% | 4 | 40 |
| Incident Response | 30% | 4 | 40 |
| Linux & Infrastructure | 15% | 3 | 30 |
| Automation & CI/CD | 10% | 2 | 20 |
| Security & Compliance | 5% | 2 | 20 |
| 24/7 Support Specific | 10% | 2 | 20 |
| Practical Skills | 10% | 2 | 20 |
| Behavioral & Situational | 5% | 2 | 20 |

**Total: 25 questions, 250 points maximum**

## Scoring Guide

- **0-2**: Poor/No understanding
- **3-4**: Basic understanding
- **5-6**: Competent
- **7-8**: Proficient
- **9-10**: Expert

## Using the System

### Candidate Navigation
- Click on candidate names to switch between interviews
- Green badges show completed questions
- Green background indicates fully completed interview

### Question Navigation
- Use **Previous/Next** buttons to navigate questions
- Progress bar shows completion percentage
- Question counter shows current position

### Scoring Each Answer
1. Ask the question to the candidate
2. Listen for key points mentioned in "Expected Answer"
3. Click a score button (0-10)
4. Add notes in the text area (optional but recommended)
5. Move to next question or candidate

### Completing Interviews
- Click **"Finish Candidate"** when all questions are answered
- System shows completion summary with total score
- Click **"Interview Next Candidate"** to continue

### Viewing Results
- Click **"View Summary"** button at any time
- See candidate rankings with percentages
- Review section-by-section breakdowns
- Export results to JSON or CSV

## Files Included

- `index.html` - Main application (open this in browser)
- `sre-interview-questions.json` - Full question set in JSON format
- `sre-interview-questions.csv` - Full question set in CSV format
- `README.md` - This documentation file

## Candidate Information

Sample candidates included:

1. **Pramod Eramudugolla**: AWS certified, current monitoring experience, 3+ years
2. **Eshani Nimeshika**: RMM platforms, PowerShell, support background, CCNA
3. **Chaveen Perera**: Current cloud monitoring (ArgoCD), Linux deployment, DevOps tools
4. **Ishara Wegapitiya**: Current DevOps role, AWS/Azure, CI/CD, Terraform, L1/L2 support

## Customization

### Creating Your Own Questions

**JSON Format:**
```json
{
  "position": "Your Position Title",
  "sections": [
    {
      "name": "Section Name",
      "weight": 25,
      "questions": [
        {
          "id": 1,
          "question": "Your question text here",
          "expectedAnswer": "Key points to look for in the answer"
        }
      ]
    }
  ]
}
```

**CSV Format:**
```csv
Section,Weight,Question,Expected Answer
"Section Name",25,"Question text","Expected answer points"
```

### Modifying Weights

Edit the `weight` field in each section to change importance. Total should equal 100%.

## Export Formats

### JSON Export
- Complete interview data with all scores and notes
- Structured format for programmatic processing
- Includes timestamps and candidate details

### CSV Export
- Spreadsheet-compatible format
- One row per question per candidate
- Includes section, question, score, and notes

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (Recommended)
- Firefox
- Safari
- Opera

## Tips for Effective Interviews

1. **Prepare**: Review questions and expected answers beforehand
2. **Be Consistent**: Ask all candidates the same questions
3. **Take Notes**: Document specific answers and observations
4. **Be Objective**: Use the scoring guide consistently
5. **Allow Time**: Let candidates think and explain their reasoning
6. **Probe Deeper**: Ask follow-up questions to assess true understanding
7. **Document**: Add notes about strengths, concerns, and specific examples

## Scoring Interpretation

### Overall Score Ranges
- **180-250 (72-100%)**: Strong Hire - Excellent technical skills
- **150-179 (60-71%)**: Hire - Solid technical foundation
- **120-149 (48-59%)**: Maybe - Some gaps, may need training
- **Below 120 (<48%)**: No Hire - Significant skill gaps

### Recommendations
Consider not just total score but also:
- Performance in critical sections (Incident Response, Monitoring)
- Cultural fit and communication skills
- Learning ability and growth mindset
- Specific role requirements

## Troubleshooting

**Questions not loading?**
- Check file format (valid JSON or CSV)
- Ensure no special characters in file name
- Try the "Load SRE Sample" button first

**Scores not saving?**
- Make sure to click score buttons
- Check browser console for errors
- Try refreshing and re-entering data

**Export not working?**
- Allow downloads in browser settings
- Check popup blocker settings
- Try different browser

## Support

For issues or questions:
1. Check this README file
2. Review the JSON format example in the app
3. Verify your question file format matches the examples

## License

Free to use and modify for your interview needs.

---

**Version**: 1.0
**Last Updated**: 2024
**Created for**: Infrastructure Support Engineer (SRE) Interviews
