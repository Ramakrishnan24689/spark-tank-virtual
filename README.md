# SparkTank UI Mockups & References

This folder contains documentation and references for the SparkTank PowerApps Code App implementation.

## UI Mockup References

The SparkTank application is based on the following UI mockups available at:

### Stage A - Team Formation
- **URL**: https://stjeffer.github.io/sparktank/ks-join-team.html
- **Description**: Workshop lobby where participants join teams
- **Key Features**: Team cards, participant assignment, readiness indicators

### Stage B - Idea Submission  
- **URL**: https://stjeffer.github.io/sparktank/ks-idea-submission.html
- **Description**: Timed idea submission with two categories
- **Key Features**: 20-minute timer, dual submission paths, facilitator oversight

### Stage C - Pitching & Voting
- **URL**: https://stjeffer.github.io/sparktank/ks-pitching-voting.html  
- **Description**: Real-time voting on team ideas
- **Key Features**: Idea cards, vote counting, winner revelation

### Stage D - Post-Workshop Summary
- **URL**: https://stjeffer.github.io/sparktank/ks-sparktank-summary.html
- **Description**: Winner package and AI-generated summaries
- **Key Features**: Structured summaries, email distribution, data export

## Implementation Notes

- These mockups are for **UI reference only**
- Implementation should use **Fluent UI v9** components for Microsoft consistency
- Focus on real-time collaboration and seamless user experience
- Maintain the workshop flow and energy of the original paper-based process

## Screen Captures

The following PNG files were referenced in the original analysis:
- `draw-cards.png` - Card-based interface elements
- `facilitator-view.png` - Facilitator dashboard overview
- `participants-view.png` - Participant interface design
- `pitching and voting.png` - Voting interface layout
- `playground-impact.png` - Impact assessment views
- `Spark-Tank.png` - Main application interface

*Note: Original PNG files were not preserved during project setup. Refer to live mockup URLs above for current UI specifications.*

## Development Guidelines

1. **Stage-by-stage Implementation**: Build and test each workshop stage independently
2. **Real-time Features**: Ensure live updates across all participant screens
3. **Mobile Responsive**: Design works on phones, tablets, and desktops
4. **Fluent UI Compliance**: Use Microsoft design language consistently
5. **Performance**: Target <3 second load times and <500ms real-time updates

## Project Structure

```
SparkTank/
├── src/
│   ├── components/          # Reusable UI components
│   ├── services/           # Data services (mock → Dataverse)
│   ├── types/              # TypeScript definitions
│   ├── contexts/           # React context providers
│   └── utils/              # Helper functions
├── public/                 # Static assets
├── Stage A-D *.md         # Original transcript files
├── requirements.md         # Complete requirements doc
└── implementation-plan.md  # Development roadmap
```

For detailed requirements and implementation guidance, see:
- `requirements.md` - Complete application specifications
- `implementation-plan.md` - Phase-by-phase development approach