# Hematology Clinical Mastery (Koas Edition)

A comprehensive web-based learning platform designed for indonesia medical students written in bahasa indonesia (co-assistants/koas) to master hematology clinical cases through interactive case-based questions.

## Overview

This application provides 300 carefully curated hematology clinical cases that simulate real-world diagnostic scenarios. Each case is designed to test clinical reasoning, diagnostic accuracy, and understanding of hematological disorders commonly encountered in medical practice.

## Features

### Interactive Learning Experience
- **300 Clinical Cases**: Comprehensive coverage of hematology topics from basic anemias to complex coagulopathies
- **Real-time Feedback**: Immediate explanations for each answer with clinical reasoning
- **Three-tier Grading System**: 
  - ✓ Correct (Benar)
  - ⚠ Close/Near (Mendekati) 
  - ✗ Incorrect (Salah)
- **Evidence-based Content**: All cases referenced from authoritative sources (Hoffbrand, Robbins)

### Progress Tracking
- **Visual Progress Indicator**: Circular progress ring showing completion percentage
- **Live Score Dashboard**: Real-time tracking of correct, near-miss, and incorrect answers
- **Performance Analytics**: End-of-session charts displaying answer distribution and overall performance

### User Interface
- **Modern Design**: Dark-themed glass-morphism interface optimized for extended study sessions
- **Responsive Layout**: Fully functional across desktop, tablet, and mobile devices
- **Smooth Animations**: Engaging transitions and visual feedback for better learning retention
- **Accessibility**: High contrast ratios and clear typography for comfortable reading

## Technical Stack

### Frontend Technologies
- **HTML5**: Semantic markup structure
- **CSS3**: Custom properties, animations, and responsive design
- **JavaScript (ES6+)**: Vanilla JS for all interactivity
- **Tailwind CSS**: Utility-first CSS framework (via CDN)
- **Chart.js**: Data visualization for performance analytics

### Design System
- **Typography**: 
  - Space Grotesk (headings)
  - Inter (body text)
- **Color Palette**:
  - Crimson Red (#dc2626) - Primary accent
  - Teal (#14b8a6) - Correct answers
  - Amber (#f59e0b) - Near-miss answers
  - Dark gradients for depth and focus

### Performance Optimizations
- **CDN Resources**: Fast loading of external libraries
- **CSS Animations**: Hardware-accelerated transforms
- **Minimal Dependencies**: Lightweight footprint for quick initialization
- **Efficient DOM Manipulation**: Optimized rendering for smooth UX

## Case Structure

Each clinical case follows a standardized format:

```javascript
{
  text: "Clinical presentation with patient demographics, symptoms, physical findings, and laboratory results",
  options: [
    {
      t: "Diagnosis option",
      s: "benar|mendekati|salah",  // grading status
      e: "Clinical explanation and reasoning",
      src: "Reference source"
    }
    // ... 4 options per case
  ]
}
```

## Coverage Areas

### Anemias
- Iron deficiency anemia
- Megaloblastic anemias (B12, folate deficiency)
- Anemia of chronic disease (ACD)
- Thalassemias (trait, major, compound heterozygous)
- Sideroblastic anemias

### Hemolytic Disorders
- Autoimmune hemolytic anemia (AIHA)
- G6PD deficiency
- Hereditary spherocytosis
- Paroxysmal nocturnal hemoglobinuria (PNH)
- Sickle cell disease

### Bone Marrow Failure
- Aplastic anemia
- Myelodysplastic syndromes (MDS)

### Coagulation Disorders
- Immune thrombocytopenia (ITP)
- Thrombotic thrombocytopenic purpura (TTP)
- Disseminated intravascular coagulation (DIC)
- Hemophilia A
- von Willebrand disease
- Vitamin K deficiency

### Malignancies
- Multiple myeloma
- Acute myeloblastic leukemia (AML)

### Complex/Mixed Cases
- Combined deficiency anemias
- Evans syndrome
- Hemoglobin variants (HbE/beta thalassemia)

## Usage

### Running Locally
1. Clone or download the repository
2. Open `index.html` in a modern web browser
3. No build process or server required - runs entirely client-side

### Deployment
The application is static and can be deployed to any web hosting platform:
- Vercel (configured via `.gitignore`)
- Netlify
- GitHub Pages
- AWS S3 + CloudFront
- Any static hosting service

## Educational Approach

### Case-Based Learning
Each case simulates real clinical encounters, requiring students to:
1. Analyze patient presentation
2. Interpret laboratory findings
3. Synthesize clinical and lab data
4. Arrive at the most likely diagnosis

### Feedback Methodology
- **Correct answers**: Reinforce understanding with pathophysiologic explanations
- **Near-miss answers**: Highlight subtle diagnostic distinctions
- **Incorrect answers**: Show the correct answer and explain common misconceptions

### Evidence-Based References
All cases cite authoritative sources:
- **Hoffbrand's Essential Haematology**: Gold standard hematology textbook
- **Robbins Pathologic Basis of Disease**: Comprehensive pathology reference

## Performance Metrics

### Session Analytics
At completion, students receive:
- **Answer Distribution Chart**: Doughnut chart showing correct/near/incorrect breakdown
- **Total Score Visualization**: Bar chart displaying overall performance
- **Completion Statistics**: Total cases attempted and accuracy rate

### Learning Outcomes
Designed to help students:
- Master diagnostic criteria for common hematologic disorders
- Differentiate between similar presentations
- Understand laboratory patterns and their clinical significance
- Build confidence for clinical rotations and examinations

## Browser Compatibility

Tested and optimized for:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## File Structure

```
hematology-test-web/
├── index.html          # Main application file (self-contained)
├── README.md           # Documentation
└── .gitignore         # Deployment configuration (Vercel)
```

## Customization

### Adding New Cases
Cases can be added to the `quizData` array following the established format:

```javascript
{
  text: "Kasus [N]: [Clinical scenario]",
  options: [
    { t: "Option text", s: "benar|mendekati|salah", e: "Explanation", src: "Reference" },
    // ... 3 more options
  ]
}
```

### Modifying Design
CSS custom properties in `:root` allow easy theme customization:
- Color scheme adjustment
- Typography changes
- Animation timing
- Component styling

## Future Enhancements

Potential features for future versions:
- Bookmark/flag difficult cases for review
- Spaced repetition algorithm for optimized learning
- Case filtering by topic/difficulty
- Export performance reports
- Multi-user support with progress persistence
- Mobile app version
- Additional question banks (oncology, coagulation deep-dive)

## License

Educational resource for medical students. Please maintain attribution to original sources (Hoffbrand, Robbins) when using or distributing.

## Acknowledgments

- **Clinical Content**: Based on established hematology principles from Hoffbrand and Robbins
- **Target Audience**: Medical co-assistants (koas) in clinical rotations
- **Design Philosophy**: Focus on learning efficiency and knowledge retention

## Support

For issues, suggestions, or contributions, please open an issue in the repository or contact the development team.

---

**Version**: 1.0  
**Last Updated**: 19 April 2026 
**Intended Use**: Educational purposes for medical students
