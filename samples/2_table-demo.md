# Table Demo

> MarkView's table rendering capabilities support various markdown table formats, including simple tables, tables with HTML content, nested lists, and complex structures.

## Test: Simple Table

| Component | Description |
|:----------|:------------|
| Kong | Work as a gateway |
| Service | Validate request |

## Test: Tables With Blank Line Between

|  A  |  B  |
|-----|-----|
| a1  | b1  |

|  C  |  D  |
|-----|-----|
| c1  | d1  |

## Test: HTML Elements in Tables

| HTML Element | Example | Rendered Output |
|:-------------|:--------|:----------------|
| Bold | `<strong>Bold text</strong>` | <strong>Bold text</strong> |
| Italic | `<em>Italic text</em>` | <em>Italic text</em> |
| Underline | `<u>Underlined text</u>` | <u>Underlined text</u> |
| Strike | `<s>Strikethrough text</s>` | <s>Strikethrough text</s> |
| Code | `<code>inline code</code>` | <code>inline code</code> |
| Subscript | `H<sub>2</sub>O` | H<sub>2</sub>O |
| Superscript | `E=mc<sup>2</sup>` | E=mc<sup>2</sup> |
| Line Break | `Line 1<br>Line 2` | Line 1<br>Line 2 |
| Small Text | `<small>Small print</small>` | <small>Small print</small> |
| Mark/Highlight | `<mark>Highlighted text</mark>` | <mark>Highlighted text</mark> |
| Keyboard | `<kbd>Ctrl</kbd> + <kbd>C</kbd>` | <kbd>Ctrl</kbd> + <kbd>C</kbd> |
| Abbreviation | `<abbr title="HyperText Markup Language">HTML</abbr>` | <abbr title="HyperText Markup Language">HTML</abbr> |

## Test: Complex HTML Structures in Tables

| Feature | Description | Example |
|:--------|:------------|:--------|
| Nested Formatting | Multiple HTML elements combined | <strong>Bold <em>and italic</em></strong> with <code>code</code> |
| Colored Text | Using inline styles | <span style="color: red;">Red</span>, <span style="color: blue;">Blue</span>, <span style="color: green;">Green</span> |
| Links with Formatting | HTML links with styling | <a href="https://example.com"><strong>Bold Link</strong></a> |
| Multiple Breaks | Multiple line breaks | First<br><br>Second<br><br>Third |
| Blockquote | Quote inside table | <blockquote>This is a quote in a table</blockquote> |
| Details/Summary | Collapsible content | <details><summary>Click to expand</summary><p>Hidden content here</p></details> |
| HTML Entities | Special characters | &copy; &trade; &reg; &hearts; &spades; |

## Test: Lists and Structured Content in Tables

| Type | Content |
|:-----|:--------|
| Simple List | <ul><li>Item 1</li><li>Item 2</li><li>Item 3</li></ul> |
| Ordered List | <ol><li>First</li><li>Second</li><li>Third</li></ol> |
| Nested List | <ul><li>Parent 1<ul><li>Child 1.1</li><li>Child 1.2</li></ul></li><li>Parent 2</li></ul> |
| Mixed Content | <p><strong>Title:</strong></p><ul><li>Point 1</li><li>Point 2</li></ul><p><em>Note: Additional info</em></p> |
| Definition List | <dl><dt>Term</dt><dd>Definition of the term</dd><dt>Another</dt><dd>Another definition</dd></dl> |

## Test: Inline Code Showing HTML Tags

| Tag | Description | Display Example |
|:----|:------------|:----------------|
| `<p>` | Paragraph tag | Used for paragraph blocks |
| `<br>` | Line break tag | Creates a line break |
| `<div>` | Division tag | Container element |
| `<span>` | Span tag | Inline container |
| `<ul>` / `<li>` | List tags | For unordered lists |
| `<strong>` | Strong tag | For bold text |
| `<em>` | Emphasis tag | For italic text |
| `<code>` | Code tag | For inline code |

## Test: HTML Attributes and Styling

| Feature | HTML Code | Result |
|:--------|:----------|:-------|
| Centered Text | `<p align="center">Centered</p>` | <p align="center">Centered</p> |
| Right Aligned | `<p align="right">Right aligned</p>` | <p align="right">Right aligned</p> |
| Font Size | `<span style="font-size: 20px;">Large</span>` | <span style="font-size: 20px;">Large</span> |
| Background Color | `<span style="background-color: yellow;">Highlighted</span>` | <span style="background-color: yellow;">Highlighted</span> |
| Custom Width | `<div style="width: 200px; border: 1px solid;">Fixed width</div>` | <div style="width: 200px; border: 1px solid;">Fixed width</div> |

## Test: Mixed Markdown and HTML

| Feature | Code | Result |
|:--------|:-----|:-------|
| Markdown + HTML | `**Bold** and <em>italic</em>` | **Bold** and <em>italic</em> |
| Link + Format | `[Link](https://example.com) with <code>code</code>` | [Link](https://example.com) with <code>code</code> |
| List Hybrid | `- Markdown item` + `<li>HTML item</li>` | - Markdown item<br><ul><li>HTML item</li></ul> |
| Code + Break | `` `inline code` <br> new line`` | `inline code` <br> new line |

## Test: Table with Internal Images

| Feature | Description | Screenshot |
|:--------|:------------|:-----------|
| Image Display | Demonstrates internal image rendering in tables | ![Internal Image](./assets/image-1.jpg) |
| Image Alignment | Shows different image alignments within table cells | <p align="center"><img src="./assets/image-2.jpg" alt="Centered Image" width="100"/></p> |
| Image with Caption | Displays an image along with a caption in a table cell | ![Image with Caption](./assets/image-3.jpg)<br>*Figure: Sample Image with Caption* |
| Linked Image | An image that acts as a hyperlink within a table cell | [![Linked Image](./assets/image-4.jpg)](https://example.com) |
| Alt Text Image | An image with alt text for accessibility | ![Alt Text Image](./assets/image-5.jpg "This is alt text for the image") |

## Test: Table Long Content

| Column 1 - Very Long Header Name | Column 2 - Another Extended Header | Column 3 - Third Long Header Title | Column 4 - Fourth Extended Column | Column 5 - Fifth Column Header | Column 6 - Sixth Column Title | Column 7 - Seventh Header Name | Column 8 - Eighth Column Header | Column 9 - Ninth Extended Header | Column 10 - Tenth Final Column |
|:----------------------------------|:------------------------------------|:-----------------------------------|:----------------------------------|:-------------------------------|:------------------------------|:-------------------------------|:--------------------------------|:---------------------------------|:-------------------------------|
| Row 1, Cell 1: This is a very long content that should force horizontal scrolling | Row 1, Cell 2: Another piece of extended content with lots of text | Row 1, Cell 3: More lengthy content to test scrolling behavior | Row 1, Cell 4: Additional long text content for testing purposes | Row 1, Cell 5: Extended content continues here | Row 1, Cell 6: More text to fill the cell | Row 1, Cell 7: Continuing with long content | Row 1, Cell 8: Additional lengthy text here | Row 1, Cell 9: More extended content for testing | Row 1, Cell 10: Final column with long text |
| Row 2, Cell 1: Lorem ipsum dolor sit amet, consectetur adipiscing elit | Row 2, Cell 2: Sed do eiusmod tempor incididunt ut labore et dolore | Row 2, Cell 3: Ut enim ad minim veniam, quis nostrud exercitation | Row 2, Cell 4: Duis aute irure dolor in reprehenderit in voluptate | Row 2, Cell 5: Excepteur sint occaecat cupidatat non proident | Row 2, Cell 6: Sunt in culpa qui officia deserunt mollit anim | Row 2, Cell 7: Et harum quidem rerum facilis est et expedita | Row 2, Cell 8: Nam libero tempore, cum soluta nobis est eligendi | Row 2, Cell 9: Temporibus autem quibusdam et aut officiis | Row 2, Cell 10: Itaque earum rerum hic tenetur a sapiente |
| Row 3, Cell 1: The quick brown fox jumps over the lazy dog multiple times | Row 3, Cell 2: Pack my box with five dozen liquor jugs repeatedly | Row 3, Cell 3: How vexingly quick daft zebras jump continuously | Row 3, Cell 4: Waltz, bad nymph, for quick jigs vex consistently | Row 3, Cell 5: Sphinx of black quartz, judge my vow repeatedly | Row 3, Cell 6: Two driven jocks help fax my big quiz extensively | Row 3, Cell 7: Five quacking zephyrs jolt my wax bed continuously | Row 3, Cell 8: The five boxing wizards jump quickly all day long | Row 3, Cell 9: How quickly daft jumping zebras vex repeatedly | Row 3, Cell 10: Quick zephyrs blow, vexing daft Jim continuously |
| Row 4, Cell 1: This row contains data about project management and coordination | Row 4, Cell 2: Information about team collaboration and communication tools | Row 4, Cell 3: Details regarding development processes and methodologies | Row 4, Cell 4: Content about quality assurance and testing procedures | Row 4, Cell 5: Documentation for deployment and release management | Row 4, Cell 6: Guidelines for code review and version control systems | Row 4, Cell 7: Specifications for performance optimization strategies | Row 4, Cell 8: Requirements for security audits and compliance checks | Row 4, Cell 9: Procedures for incident response and troubleshooting | Row 4, Cell 10: Policies for user feedback and continuous improvement |
| Row 5, Cell 1: Advanced configuration settings for the application framework | Row 5, Cell 2: Detailed analysis of system architecture and design patterns | Row 5, Cell 3: Comprehensive overview of database schema and relationships | Row 5, Cell 4: In-depth explanation of API endpoints and authentication | Row 5, Cell 5: Technical documentation for third-party integrations | Row 5, Cell 6: Performance metrics and monitoring dashboard configurations | Row 5, Cell 7: Detailed logging and error tracking implementation details | Row 5, Cell 8: Scalability considerations and load balancing strategies | Row 5, Cell 9: Caching mechanisms and optimization techniques explained | Row 5, Cell 10: Backup and disaster recovery procedures documentation |
| Row 6, Cell 1: User interface components and responsive design considerations | Row 6, Cell 2: Frontend framework integration and state management patterns | Row 6, Cell 3: Cross-browser compatibility testing and validation results | Row 6, Cell 4: Accessibility standards compliance and WCAG guidelines | Row 6, Cell 5: Internationalization and localization support documentation | Row 6, Cell 6: Theme customization and branding configuration options | Row 6, Cell 7: Animation and transition effects implementation details | Row 6, Cell 8: Form validation and user input sanitization procedures | Row 6, Cell 9: Progressive web app features and offline functionality | Row 6, Cell 10: Mobile-first design approach and responsive breakpoints |
| Row 7, Cell 1: Backend service architecture and microservices communication | Row 7, Cell 2: Message queue implementation and asynchronous processing | Row 7, Cell 3: RESTful API design principles and best practices followed | Row 7, Cell 4: GraphQL schema definition and query optimization techniques | Row 7, Cell 5: WebSocket implementation for real-time data transmission | Row 7, Cell 6: Server-side rendering and static site generation methods | Row 7, Cell 7: Content delivery network configuration and edge caching | Row 7, Cell 8: Database query optimization and indexing strategies used | Row 7, Cell 9: Transaction management and data consistency guarantees | Row 7, Cell 10: Event-driven architecture and event sourcing patterns |
| Row 8, Cell 1: Continuous integration and continuous deployment pipelines | Row 8, Cell 2: Automated testing frameworks and test coverage requirements | Row 8, Cell 3: Docker containerization and orchestration with Kubernetes | Row 8, Cell 4: Infrastructure as code using Terraform and cloud resources | Row 8, Cell 5: Monitoring and alerting systems with Prometheus and Grafana | Row 8, Cell 6: Log aggregation and analysis using ELK stack components | Row 8, Cell 7: Secret management and credential storage best practices | Row 8, Cell 8: Network security and firewall configuration guidelines | Row 8, Cell 9: SSL/TLS certificate management and HTTPS enforcement | Row 8, Cell 10: Rate limiting and DDoS protection implementation details |
| Row 9, Cell 1: Data privacy regulations and GDPR compliance requirements | Row 9, Cell 2: User consent management and cookie policy implementation | Row 9, Cell 3: Data encryption at rest and in transit using modern algorithms | Row 9, Cell 4: Authentication mechanisms including OAuth 2.0 and SAML | Row 9, Cell 5: Multi-factor authentication setup and security token usage | Row 9, Cell 6: Role-based access control and permission management system | Row 9, Cell 7: Audit logging and compliance reporting functionalities | Row 9, Cell 8: Penetration testing results and vulnerability assessments | Row 9, Cell 9: Security incident response plan and escalation procedures | Row 9, Cell 10: Regular security updates and patch management schedules |
| Row 10, Cell 1: Customer relationship management and support ticketing system | Row 10, Cell 2: Email marketing automation and campaign management tools | Row 10, Cell 3: Analytics and reporting dashboards with custom visualizations | Row 10, Cell 4: A/B testing framework for feature experimentation and analysis | Row 10, Cell 5: Search engine optimization strategies and meta tag management | Row 10, Cell 6: Social media integration and sharing functionality features | Row 10, Cell 7: Payment gateway integration and transaction processing | Row 10, Cell 8: Subscription management and recurring billing implementation | Row 10, Cell 9: Inventory management and order fulfillment workflows | Row 10, Cell 10: Customer feedback collection and survey distribution |
| Row 11, Cell 1: Machine learning model training and deployment infrastructure | Row 11, Cell 2: Data pipeline orchestration and ETL process automation | Row 11, Cell 3: Feature engineering and data preprocessing techniques used | Row 11, Cell 4: Model versioning and experiment tracking with MLflow setup | Row 11, Cell 5: Hyperparameter tuning and automated model selection methods | Row 11, Cell 6: Model serving and inference API endpoint configurations | Row 11, Cell 7: A/B testing for ML models and champion-challenger framework | Row 11, Cell 8: Model monitoring and drift detection alert mechanisms | Row 11, Cell 9: Explainability and interpretability tools for predictions | Row 11, Cell 10: Bias detection and fairness evaluation in ML systems |
| Row 12, Cell 1: Content management system features and editorial workflows | Row 12, Cell 2: Media library organization and digital asset management | Row 12, Cell 3: Version control for content and revision history tracking | Row 12, Cell 4: Workflow automation and approval processes for publishing | Row 12, Cell 5: Multi-channel content distribution and syndication setup | Row 12, Cell 6: SEO-friendly URL structures and permalink configurations | Row 12, Cell 7: Rich text editor customization and formatting options | Row 12, Cell 8: Template management and reusable content components | Row 12, Cell 9: Scheduled publishing and content expiration functionalities | Row 12, Cell 10: Content personalization and audience segmentation rules |
| Row 13, Cell 1: Mobile application development using React Native framework | Row 13, Cell 2: Native module integration and platform-specific code handling | Row 13, Cell 3: Push notification implementation with Firebase Cloud Messaging | Row 13, Cell 4: Offline-first architecture and local data synchronization | Row 13, Cell 5: In-app purchases and subscription management for mobile apps | Row 13, Cell 6: Deep linking and universal links configuration for navigation | Row 13, Cell 7: App performance optimization and memory management techniques | Row 13, Cell 8: Crash reporting and error tracking with Sentry integration | Row 13, Cell 9: App store optimization strategies and metadata management | Row 13, Cell 10: Beta testing distribution through TestFlight and Play Store |
| Row 14, Cell 1: Real-time collaboration features using operational transform | Row 14, Cell 2: Conflict resolution strategies for concurrent editing sessions | Row 14, Cell 3: Presence indicators and user activity tracking mechanisms | Row 14, Cell 4: Chat and messaging functionality with emoji support included | Row 14, Cell 5: File sharing and collaborative document editing capabilities | Row 14, Cell 6: Video conferencing integration with WebRTC technologies | Row 14, Cell 7: Screen sharing and remote assistance features implemented | Row 14, Cell 8: Whiteboard and drawing tools for visual collaboration | Row 14, Cell 9: Task assignment and project management collaboration features | Row 14, Cell 10: Comment threads and discussion forums for team communication |
| Row 15, Cell 1: Blockchain integration and cryptocurrency payment processing | Row 15, Cell 2: Smart contract development and deployment on Ethereum network | Row 15, Cell 3: NFT minting and marketplace functionality implementation | Row 15, Cell 4: Decentralized identity management and self-sovereign identity | Row 15, Cell 5: Distributed ledger technology for supply chain tracking | Row 15, Cell 6: Consensus mechanisms and proof-of-stake validation protocols | Row 15, Cell 7: Crypto wallet integration and secure key management systems | Row 15, Cell 8: Token economics and governance mechanisms for DAOs | Row 15, Cell 9: Layer 2 scaling solutions and gas optimization strategies | Row 15, Cell 10: Cross-chain bridges and interoperability protocols enabled |
| Row 16, Cell 1: Internet of Things device connectivity and protocol support | Row 16, Cell 2: Sensor data collection and real-time telemetry processing | Row 16, Cell 3: Edge computing capabilities and fog computing architecture | Row 16, Cell 4: Device provisioning and lifecycle management automation | Row 16, Cell 5: Over-the-air firmware updates and remote device configuration | Row 16, Cell 6: Predictive maintenance using sensor data and ML algorithms | Row 16, Cell 7: Energy optimization and power management for IoT devices | Row 16, Cell 8: Geolocation tracking and asset monitoring functionalities | Row 16, Cell 9: Industrial automation and SCADA system integration points | Row 16, Cell 10: Smart home integration with voice assistants and hubs |
| Row 17, Cell 1: Augmented reality features using ARKit and ARCore frameworks | Row 17, Cell 2: 3D model rendering and manipulation in virtual environments | Row 17, Cell 3: Gesture recognition and interaction design for AR experiences | Row 17, Cell 4: Spatial mapping and environment understanding capabilities | Row 17, Cell 5: Marker-based and markerless tracking implementation methods | Row 17, Cell 6: Virtual try-on and product visualization for e-commerce | Row 17, Cell 7: AR navigation and wayfinding assistance applications | Row 17, Cell 8: Collaborative AR experiences and multi-user synchronization | Row 17, Cell 9: Image recognition and object detection in AR contexts | Row 17, Cell 10: Performance optimization for mobile AR applications |
| Row 18, Cell 1: Voice user interface and natural language processing features | Row 18, Cell 2: Speech recognition and transcription service integration | Row 18, Cell 3: Text-to-speech synthesis with multiple language support | Row 18, Cell 4: Intent recognition and entity extraction for conversational AI | Row 18, Cell 5: Chatbot development and dialogue management frameworks used | Row 18, Cell 6: Sentiment analysis and emotion detection in text and voice | Row 18, Cell 7: Voice biometrics and speaker identification capabilities | Row 18, Cell 8: Multi-turn conversation handling and context management | Row 18, Cell 9: Voice command execution and smart assistant integration | Row 18, Cell 10: Noise cancellation and audio signal processing techniques |
| Row 19, Cell 1: Gamification elements and achievement system implementation | Row 19, Cell 2: Leaderboards and competitive ranking mechanisms configured | Row 19, Cell 3: Points, badges, and rewards distribution automation system | Row 19, Cell 4: Progress tracking and milestone celebration features added | Row 19, Cell 5: Challenge and quest systems for user engagement strategies | Row 19, Cell 6: Social features and friend invitation mechanics implemented | Row 19, Cell 7: Daily streaks and login reward mechanisms to boost retention | Row 19, Cell 8: Virtual currency and in-game economy balance management | Row 19, Cell 9: Avatar customization and personalization options provided | Row 19, Cell 10: Tournament and event management for competitive gameplay |
| Row 20, Cell 1: Accessibility features including screen reader compatibility | Row 20, Cell 2: Keyboard navigation and focus management implementations | Row 20, Cell 3: High contrast themes and color blindness accommodation modes | Row 20, Cell 4: Text resizing and zoom functionality for better readability | Row 20, Cell 5: Closed captions and audio descriptions for media content | Row 20, Cell 6: Alternative text for images and descriptive link text usage | Row 20, Cell 7: ARIA labels and semantic HTML for assistive technologies | Row 20, Cell 8: Voice control and switch control support for motor disabilities | Row 20, Cell 9: Reduced motion options and animation preferences respected | Row 20, Cell 10: Form error messages and clear instructions for accessibility |
