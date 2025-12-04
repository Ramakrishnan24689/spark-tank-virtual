# SparkTank PowerApps Code App - Requirements Document

## Overview
SparkTank is an interactive innovation platform designed to facilitate AI-driven ideation sessions. The platform enables teams to collaboratively generate, pitch, and vote on AI use cases in a structured workshop environment.

## Business Context
SparkTank transforms traditional brainstorming sessions into structured digital workshops where participants can:
- Form dynamic teams
- Submit AI-focused improvement ideas
- Pitch concepts to teammates
- Vote on the most impactful ideas
- Select winning concepts for further development

## User Personas

### 1. Facilitator (Administrator)
**Role**: Workshop organizer and moderator
**Responsibilities**:
- Set up workshop sessions and teams
- Monitor real-time participation across all teams
- Manage timers for each stage
- View all submitted ideas and voting progress
- Control stage transitions
- Reveal final results

**Key Needs**:
- Real-time dashboard visibility
- Team management capabilities
- Session control and timing
- Comprehensive reporting

### 2. Participant (End User)
**Role**: Workshop attendee and idea contributor
**Responsibilities**:
- Join or create teams
- Submit improvement ideas
- Listen to team pitches
- Vote on preferred concepts
- Collaborate within assigned team

**Key Needs**:
- Simple team selection
- Intuitive idea submission
- Clear voting interface
- Real-time feedback

### Stage D: SparkTank Card Activity
**Duration**: 30-40 minutes (guided card analysis)
**Objective**: Build comprehensive use case framework through structured card analysis

**Facilitator View Features**:
- **Timer Control**: 
  - 30-40 minute countdown with pause/reset
  - Card draw pace guidance (1 minute per card)
- **Card Deck Management**:
  - Digital card deck with 5 categories
  - "Draw Card" button for controlled card revelation
  - Remaining cards counter
- **Team Progress Monitor**:
  - Real-time view of each team's card assignments
  - Playbook completion status per team
  - AI generation progress indicators
- **AI Assistant Controls**:
  - "Generate AI Insights" for incomplete sections
  - Batch playbook generation across all teams
  - Quality review and approval workflow

**Participant View Features**:
- **Card Canvas Interface**:
  - 5-zone canvas: Stakeholders, Objectives, Challenges, Outcomes, Wildcard Zone
  - Drag-and-drop card placement system
  - Category-specific classification (Critical, Influential, Not Relevant)
- **Interactive Card Analysis**:
  - **Stakeholders Zone**: 
    - Cards: Manager, IT Administrator, Change Manager, End User, Customer/Client, Partner/Supplier, Process Owner
    - Classification: Critical, Influential, Not Relevant to Use Case
  - **Objectives Zone**:
    - Cards: Improve Efficiency, Enhance User Experience, Ensure Compliance, Improve Collaboration, Reduce Costs, Increase Revenue, Scale Operations
    - Classification: Primary, Secondary, Not Relevant
  - **Challenges Zone**:
    - Cards: User Adoption Resistance, Data Quality Issues, Integration Complexity, Data Privacy, Regulatory Compliance, Technical Debt
    - Impact Assessment: High Impact, Manageable, Not Relevant
  - **Outcomes Zone**:
    - Cards: Improved Employee Satisfaction, Automate Repetitive Tasks, Reduce Response Times, Optimize Workflow, Cost Savings
    - Classification: Essential, Beneficial, Not Relevant
    - Measurement Method Selection: Surveys, Analytics, Telemetry, KPI Tracking
  - **Wildcard Zone**:
    - Randomized constraint cards: Employee Mistrust, Competition Launches Similar Solution, High Staff Turnover, Budget Constraints, Technology Changes
    - Impact Assessment: Critical Impact, Manageable, Not Relevant

**AI-Powered Playbook Generation**:
- **Why Stakeholders Critical**: AI explains relevance of classified stakeholders to use case
- **Why Objectives Important**: AI generates rationale for primary/secondary objective prioritization
- **Challenge Mitigation**: AI proposes strategies for managing high-impact challenges
- **Outcome Measurement**: AI suggests specific measurement methods and KPIs for each outcome
- **Wildcard Integration**: AI helps teams incorporate constraint cards into their use case planning

**Key Requirements**:
- Digital card deck with 40+ cards across 5 categories
- Intuitive drag-and-drop classification interface
- Real-time AI content generation
- Structured playbook output format
- Team collaboration features within card canvas
- Export capabilities for completed playbooks

### Stage E: Post-Workshop Summary
**Duration**: Post-workshop activity
**Objective**: Provide comprehensive results and actionable takeaways

**Facilitator View Features**:
- **Winner Package Display**:
  - Complete winning idea summary with structured format
  - Objectives, stakeholders, challenges, and expected outcomes
  - "Email summary to winner" functionality
- **AI Summary Generation**:
  - "Generate AI Summary" button for all non-winning ideas
  - Automated compilation of insights from all submissions
  - Batch email distribution to all participants
- **Data Export Capabilities**:
  - Export anonymized use case data (excluding usernames)
  - Capture TPID and structured idea information
  - Generate reports for organizational learning

**Participant View Features**:
- **Personal Results Access**:
  - View detailed winning idea package
  - Access to their own submitted ideas
  - Email delivery option for personal copy
- **Summary Reception**:
  - Receive AI-generated summary of all workshop ideas
  - Structured takeaway materials for future reference
  - Learning framework for use case development

**Key Requirements**:
- Comprehensive winner documentation
- AI-powered insight generation
- Privacy-compliant data handling
- Actionable takeaway materials
- Email distribution system

## Application Stages

### Stage A: Team Formation
**Duration**: Setup phase
**Objective**: Organize participants into collaborative teams

**Facilitator View Features**:
- **Team Cards Display**: Visual cards showing team details
  - Team name (e.g., "Table 1 - Finance")
  - Participant count with status indicator
  - "Ready" status when team has participants
  - "Waiting" status for empty teams
- **Participants Panel**: Shows unassigned participants
  - Drag-and-drop assignment capability
  - Dropdown-based assignment as fallback
  - "Quick add participant" functionality
- **Readiness Indicator**: Overall workshop readiness status
  - Shows "X of Y teams have at least one participant"
  - "Start workshop" button (enabled when ready)
- Real-time updates across all views

**Participant View Features**:
- **Name Selection**: Dropdown or manual entry
- **Team Selection Interface**: 
  - Visual team cards with current member count
  - Team names and descriptions
  - Real-time occupancy updates
  - One-click joining functionality
- **Status Display**: Clear indication of current team assignment
- **Lobby View**: Waiting area before team assignment

**Key Requirements**:
- Dynamic team creation
- Real-time participant updates
- Flexible team size management
- Clear visual team representation

### Stage B: Idea Submission
**Duration**: 20 minutes (timed)
**Objective**: Generate and collect AI improvement ideas

**Facilitator View Features**:
- **Timer Control**: 
  - Digital countdown display (format: MM:SS)
  - Pause and Reset controls
  - 20-minute default duration
- **Team Overview Cards**:
  - Team name and focus area
  - Idea count with puzzle piece icon
  - "View Ideas" action button
- **Idea Management**:
  - Individual idea selection and viewing
  - Edit unlock functionality for participants
  - Real-time submission tracking

**Participant View Features**:
- Two idea categories:
  1. **Build Something Better**: Improve existing processes
  2. **Build Better Things**: Create new capabilities

**Idea Submission Forms**:

**Build Something Better**:
- Process/task identification
- Current process description
- AI assistance opportunities
- Expected impact assessment

**Build Better Things**:
- Strategic goal/opportunity definition
- Beneficiary identification
- AI enablement description
- New capability impact

**Key Requirements**:
- Timed submission window
- Category-based idea capture
- Real-time idea visibility
- Edit capability with facilitator control
- Multiple ideas per participant support

### Stage C: Pitching & Voting
**Duration**: Pitching period + voting window
**Objective**: Present ideas and select winning concepts

**Facilitator View Features**:
- **Timer & Controls**:
  - Countdown timer with Pause/Reset
  - "Reveal winners" button
- **Team Voting Dashboard**:
  - Team cards showing "X ideas pitched"
  - Individual idea cards displaying:
    - Idea title and brief description
    - Submitter name
    - Real-time vote count
  - Visual vote count indicators
- **Results Management**:
  - Ability to reveal winners across all teams
  - Clear winner identification per team

**Participant View Features**:
- **Idea Display**:
  - Team's submitted ideas in card format
  - Idea titles with brief descriptions
  - Submitter identification
- **Voting Interface**:
  - One-click voting buttons
  - Real-time vote count updates
  - Visual feedback on vote submission
- **Team Focus**: Only vote within assigned team's ideas

**Key Requirements**:
- Secure voting mechanism
- Real-time vote aggregation
- Clear winner identification
- Team-based result organization

## Proposed Dataverse Data Model

### 1. Workshop Session (sparktank_session)
**Purpose**: Master record for each workshop instance
```
- SessionId (Primary Key)
- SessionName (Text)
- SessionDate (DateTime)
- FacilitatorId (Lookup to User)
- Status (Choice: Setup, Team Formation, Idea Submission, Pitching/Voting, SparkTank Cards, Completed)
- CurrentStage (Choice: A, B, C, D, E)
- IdeaSubmissionTimer (Number - minutes)
- CreatedOn (DateTime)
- ModifiedOn (DateTime)
```

### 2. Team (sparktank_team)
**Purpose**: Workshop team information
```
- TeamId (Primary Key)
- SessionId (Lookup to sparktank_session)
- TeamName (Text)
- TeamColor (Text)
- MaxMembers (Number)
- CreatedBy (Lookup to User)
- CreatedOn (DateTime)
```

### 3. Participant (sparktank_participant)
**Purpose**: Workshop attendee records
```
- ParticipantId (Primary Key)
- SessionId (Lookup to sparktank_session)
- TeamId (Lookup to sparktank_team)
- UserName (Text)
- Email (Email)
- JoinedAt (DateTime)
- IsPresent (Yes/No)
```

### 4. SparkTank Card (sparktank_card)
**Purpose**: Master card deck for workshop activities
```
- CardId (Primary Key)
- CardName (Text)
- CardCategory (Choice: Stakeholders, Objectives, Challenges, Outcomes, Wildcard)
- CardDescription (Multiple Lines of Text)
- CardType (Text) - specific card type within category
- IsActive (Yes/No)
- SortOrder (Number)
```

### 5. Team Card Assignment (sparktank_teamcard)
**Purpose**: Cards drawn/assigned to each team
```
- AssignmentId (Primary Key)
- SessionId (Lookup to sparktank_session)
- TeamId (Lookup to sparktank_team)
- CardId (Lookup to sparktank_card)
- Classification (Text) - Critical/Influential/Primary/etc based on card category
- Impact (Text) - High/Manageable/etc for challenge cards
- AssignedAt (DateTime)
- IsAnalyzed (Yes/No)
```

### 6. Playbook (sparktank_playbook)
**Purpose**: AI-generated explanations and strategies
```
- PlaybookId (Primary Key)
- SessionId (Lookup to sparktank_session)
- TeamId (Lookup to sparktank_team)
- SectionType (Choice: Stakeholders, Objectives, Challenges, Outcomes, Wildcard)
- AIGeneratedContent (Multiple Lines of Text)
- UserModifications (Multiple Lines of Text)
- IsAIGenerated (Yes/No)
- IsCompleted (Yes/No)
- GeneratedAt (DateTime)
- ModifiedAt (DateTime)
```

### 7. Idea (sparktank_idea)
**Purpose**: Submitted improvement concepts
```
- IdeaId (Primary Key)
- SessionId (Lookup to sparktank_session)
- TeamId (Lookup to sparktank_team)
- SubmittedBy (Lookup to sparktank_participant)
- IdeaCategory (Choice: Build Something Better, Build Better Things)
- IdeaTitle (Text)
- ProcessTask (Text)
- Description (Multiple Lines of Text)
- AIAssistance (Multiple Lines of Text)
- ExpectedImpact (Multiple Lines of Text)
- StrategicGoal (Text) - for "Build Better Things"
- Beneficiaries (Text) - for "Build Better Things"
- NewCapability (Multiple Lines of Text) - for "Build Better Things"
- SubmittedAt (DateTime)
- IsEditable (Yes/No)
- VoteCount (Number)
- IsWinner (Yes/No)
```

### 8. Vote (sparktank_vote)
**Purpose**: Voting records for ideas
```
- VoteId (Primary Key)
- SessionId (Lookup to sparktank_session)
- IdeaId (Lookup to sparktank_idea)
- VotedBy (Lookup to sparktank_participant)
- VotedAt (DateTime)
```

### 9. Session Stage (sparktank_sessionstage)
**Purpose**: Stage timing and control
```
- StageId (Primary Key)
- SessionId (Lookup to sparktank_session)
- StageCode (Choice: A, B, C, D, E)
- StageName (Text)
- StartTime (DateTime)
- EndTime (DateTime)
- Duration (Number - minutes)
- IsActive (Yes/No)
```

## Detailed UI Specifications (Based on GitHub Mockups)

### Stage A: Team Formation UI Elements
- **Workshop Lobby Interface**
- **Team Cards**: Visual representation with team names, participant counts, and status
- **Readiness Indicator**: "X of Y teams have at least one participant" status
- **Participant Management**: Unassigned participants list with quick-add functionality
- **Start Workshop Button**: Enabled when minimum readiness criteria met

### Stage B: Idea Submission UI Elements
- **20-minute Timer**: MM:SS countdown with pause/reset controls
- **Team Overview**: Cards showing idea count with puzzle piece icons
- **View Ideas**: Action buttons for each team
- **Multi-idea Support**: Participants can submit multiple ideas
- **Unlock Edit Workflow**: Facilitator can unlock ideas for editing

### Stage C: Pitching & Voting UI Elements
- **Pitch Cards**: Individual idea displays with:
  - Idea title and brief description
  - Submitter name clearly displayed
  - Real-time vote counter
- **Team Sections**: Organized by table/team with idea counts
- **Voting Controls**: Simple click-to-vote interface
- **Reveal Winners**: Facilitator-controlled results revelation
- **Example Ideas from Mockup**:
  - "Automated invoice matching" (3 votes)
  - "Forecast assistant" (1 vote)
  - "Agent assist for tier 1" (2 votes)

### Stage D: SparkTank Card Activity UI Elements
- **Card Canvas**: 5-zone layout with color-coded sections
  - Blue: Stakeholders zone
  - Green: Objectives zone  
  - Orange: Challenges zone
  - Purple: Outcomes zone
  - Gray: Wildcard zone
- **Card Deck Interface**: 
  - "Draw Card" button with remaining count
  - Card categories and descriptions
  - Timer display for pacing
- **Classification Controls**:
  - Radio buttons for card categorization
  - Drag-and-drop card placement
  - Text areas for explanations
- **AI Playbook Generation**:
  - "Generate AI Insights" buttons per section
  - Editable AI-generated content areas
  - Save and export playbook functionality
- **Team Collaboration**:
  - Shared canvas view for team members
  - Real-time updates across team devices
  - Discussion notes and annotations

### 10. Summary Package (sparktank_summary)
**Purpose**: Post-workshop results and AI-generated insights
```
- SummaryId (Primary Key)
- SessionId (Lookup to sparktank_session)
- IdeaId (Lookup to sparktank_idea) - for winner
- SummaryType (Choice: Winner Package, AI Summary)
- Title (Text)
- Objectives (Multiple Lines of Text)
- Stakeholders (Multiple Lines of Text)
- Challenges (Multiple Lines of Text)
- ExpectedOutcomes (Multiple Lines of Text)
- ValueProposition (Multiple Lines of Text)
- AIGeneratedContent (Multiple Lines of Text)
- CreatedOn (DateTime)
- EmailSent (Yes/No)
- EmailSentTo (Multiple Lines of Text)
```

### 11. Export Data (sparktank_export)
**Purpose**: Anonymized data export for organizational insights
```
- ExportId (Primary Key)
- SessionId (Lookup to sparktank_session)
- ExportType (Choice: Full Summary, Anonymized Data)
- ExportData (Multiple Lines of Text)
- GeneratedOn (DateTime)
- GeneratedBy (Lookup to User)
- IncludesPII (Yes/No)
```

## Technical Requirements

### Frontend Components
- **Dashboard Views**: Dual-view architecture (facilitator/participant)
- **Real-time Updates**: Live data synchronization using SignalR or similar
- **Timer Component**: 
  - MM:SS format countdown display
  - Pause/Reset functionality
  - Stage-specific timing
- **Card-based UI**: Consistent card design for teams and ideas
- **Status Indicators**: Visual readiness and progress indicators
- **Responsive Design**: Mobile and desktop compatibility
- **Progressive Web App**: Offline capability considerations
- **Interactive Elements**: Drag-and-drop, one-click actions, dropdown selectors

### Integration Points
- **Microsoft 365**: User authentication and profile integration
- **Teams Integration**: Workshop notifications and updates
- **Power Automate**: Automated session management workflows
- **Power BI**: Analytics and reporting dashboards

### Security & Compliance
- **Role-based Access**: Facilitator vs. participant permissions
- **Data Privacy**: Session data isolation
- **Audit Trail**: Complete activity logging
- **Authentication**: Azure AD integration

## Success Criteria
1. Seamless team formation with real-time updates
2. Efficient 20-minute idea collection with timer management
3. Engaging pitching and voting experience
4. Clear winner identification and results presentation
5. Complete session data capture for analysis
6. Intuitive user experience requiring minimal training

## Implementation Phases
1. **Phase 1**: Team formation and idea submission (Stages A & B)
2. **Phase 2**: Voting mechanism and real-time updates (Stage C) 
3. **Phase 3**: SparkTank card activity and AI playbook generation (Stage D)
4. **Phase 4**: Post-workshop summary and AI insights (Stage E)
5. **Phase 5**: Analytics, reporting, and Teams integration

This requirements document provides the foundation for developing a comprehensive SparkTank PowerApps Code App that delivers an engaging, efficient, and results-driven innovation workshop experience with complete follow-through and actionable outcomes.
