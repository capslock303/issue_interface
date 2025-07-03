# TCPA Violation Evaluator

A comprehensive web-based interface for evaluating potential violations of the Telephone Consumer Protection Act (TCPA), specifically 47 U.S.C. § 227(b)(1)(A)(iii).

## Overview

This tool provides an interactive, step-by-step evaluation process to determine whether a TCPA violation has occurred. It guides users through a series of user-friendly yes/no questions based on the legal requirements of the TCPA, making complex legal concepts accessible to everyone.

## Features

- **Interactive Flow**: Step-by-step question flow with immediate feedback
- **Modern UI**: Clean, responsive design that works on desktop and mobile devices
- **Progress Tracking**: Visual progress bar showing evaluation completion
- **Detailed Explanations**: Comprehensive explanations for each outcome
- **Legal Accuracy**: Based on actual TCPA statutory requirements
- **Restart Functionality**: Easy restart for new evaluations

## How to Use

1. **Open the Interface**: Open `index.html` in any modern web browser
2. **Answer Questions**: Click "Yes" or "No" for each question as it appears
3. **Review Results**: Get immediate feedback with detailed explanations
4. **Start Over**: Use the "Start New Evaluation" button to begin a new assessment

## Question Flow

The evaluation follows this exact sequence:

### 1. Did you receive a call or text from a number you did not recognize?
- **Yes** → Continue to question 2
- **No** → No violation (no call/text occurred)

### 2. Was the call/text on your personal phone number?
- **Yes** → Continue to question 3
- **No** → Not covered under this subsection (landline calls covered under different provisions)

### 3. Did the caller use an artificial or prerecorded voice?
- **Yes** → Continue to question 4
- **No** → Not covered under this subsection (manual calls not covered)

### 4. Was the call made for emergency purposes?
- **Yes** → Exception - No violation (emergency calls exempt)
- **No** → Continue to question 5

### 5. Had you previously given consent to receive the call/text?
- **Yes** → Exception - No violation (consent is complete defense)
- **No** → Continue to question 6

### 6. Are you the person listed as the regular user of the phone number that was called?
- **Yes** → Violation established (all elements met)
- **No** → Might not have standing (standing issue)

## Legal Basis

This tool is based on **47 U.S.C. § 227(b)(1)(A)(iii)**, which prohibits:

> "any call (other than a call made for emergency purposes or made with the prior express consent of the called party) using any automatic telephone dialing system or an artificial or prerecorded voice... to any telephone number assigned to a paging service, cellular telephone service, specialized mobile radio service, or other radio common carrier service, or any service for which the called party is charged for the call"

## Outcome Categories

- **Violation Established**: All elements of TCPA violation met
- **No Violation**: No call/text occurred
- **Exception - No Violation**: Emergency purposes or prior express consent
- **Not Covered Under This Subsection**: Landline calls or manual dialing
- **Might Not Have Standing**: Plaintiff may lack standing to sue

## Technical Details

- **Pure HTML/CSS/JavaScript**: No external dependencies required
- **Responsive Design**: Works on all device sizes
- **Modern CSS**: Uses gradients, animations, and modern styling
- **Accessibility**: High contrast colors and clear typography

## File Structure

```
issue_interface/
├── index.html          # Main interface file
└── README.md          # This documentation file
```

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with JavaScript enabled

## Legal Disclaimer

This tool is for educational and informational purposes only. It should not be considered legal advice. For legal matters, consult with a qualified attorney. The evaluation is based on general TCPA principles and may not account for all specific circumstances or recent case law developments.

## Usage Instructions

1. Download or clone this repository
2. Open `index.html` in your web browser
3. Follow the prompts to evaluate your TCPA situation
4. Review the detailed explanation of your result
5. Use the restart button for additional evaluations

## Customization

The interface can be easily customized by modifying the HTML, CSS, or JavaScript in the `index.html` file. The question flow, styling, and logic can all be adjusted as needed. 