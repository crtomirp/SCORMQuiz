# SCORMQuiz

SCORMQuiz is a versatile, "Who Wants to Be a Millionaire" style quiz application, crafted with educational purposes in mind. It's designed for easy integration with SCORM-compliant Learning Management Systems (LMS), such as Open edX. Written in JavaScript, this responsive quiz platform is simple to customize, making it a perfect fit for any educational content.

## Customizing SCORMQuiz

### Modifying Quiz Content

#### Questions and Answers

Edit the `questions.json` file to update or add new quiz content. Here's an example entry:

```json
[
  {
    "question": "What is the capital of France?",
    "figure": "img/paris.png",
    "answers": ["Paris", "London", "Berlin", "Madrid"],
    "correct": "Paris"
  }
  // Add more questions here
]
```

#### Images

To add visual elements, place images in the `img` folder and reference them in your `questions.json`.

#### Styling

Customize the appearance by modifying `style.css`. Adjust fonts, colors, button styles, etc., to align with your branding.

### Extending Functionality

- **Adding New Question Types**: Implement different question formats by editing the main JavaScript file and adapting the `questions.json`.
- **SCORM Integration Enhancements**: For additional SCORM functionalities, adjust the SCORM script files to meet specific learner data reporting needs.

## Uploading to a SCORM System (Open edX)

### Package Your Quiz

Use a SCORM packaging tool to create a SCORM-compliant package including all necessary files and `imsmanifest.xml`.

### Test Your Package

Ensure compatibility by testing your package with a SCORM player or debugger.

### Upload to Open edX

- Log into Open edX studio and navigate to your course.
- Add a new unit, select "Advanced", and choose "SCORM".
- Upload the SCORM package and configure as needed.

### Publish

With your SCORMQuiz uploaded and configured, publish your course for learner access.

## Conclusion

SCORMQuiz offers an engaging way to incorporate interactive quizzes into e-learning, easily tailored to fit unique educational needs. Happy quizzing!
