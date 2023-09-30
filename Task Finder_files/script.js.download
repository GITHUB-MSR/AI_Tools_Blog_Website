 
 src="https://cdn.jsdelivr.net/npm/fuse.js"
        const data = [
            {
                tags: "presenatations,ppt,presentation,project,slide,word,document,ai",
            },
            {
                tags: "resume,image,images,design,desings,art,cv",
            },
            {
                tags: "spelling,check,grammar,essay,english,vocabulary,ai",
            },
            {
                tags:"code,Coding,program,chat, Languages, Software development, Coding tips and tricks, computer,computer science, Music, Guitar, piano, bass guitar, Music composition, Music theory, Favorite music genres, Space and Science, Astronomy, Space exploration, Physics, Scientific discoveries, Cars and Retro Bikes, Car models, Vintage motorcycles, Automotive technology, Restoration projects, Career Goals, Job search strategies, Software industry insights, Career development advice, Maximizing income potential, Family and Goals, Overcoming poverty, Family well-being, Financial planning, Achieving personal goals",
            },
            {
                tags:"Notion, Productivity tool, Note-taking, Task management, Project planning, All-in-one workspace, Pages, Blocks, Templates, Collaboration, Databases, Relations, Formulas, Integration, Mobile app, Customization, Organization, Productivity, Workflow, Note organization, Task tracking",
            },
            {
                tags:"trello, Project management, Task tracking, Kanban boards, Cards, Lists, Boards, Labels, Due dates, Collaboration, Workflow, Productivity tool, Customization, Integrations, Mobile app, Team collaboration, Project organization",
            },
            {
                   tags:"Otter.ai, Transcription, Note-taking, Speech-to-text, Meetings, Interviews, Voice recordings, Automatic transcription, Collaboration, Searchable notes, Integration, Productivity tool, Mobile app,audio files, Text synchronization, Meeting minutes",
            },
            {
                tags:"Prezi, Presentation, Visuals, Slides, Templates, Zooming, Animation, Design, Storytelling, Engagement, Collaboration",
            },
            {
                tags:"Anki, Flashcards, Spaced repetition, Memorization, Study, Cards, Decks, Learning, Synchronization, Mobile app, Customization, Review, Active recall, Language learning, Exam preparation",
            },
            {
                tags:"Turnitin, Plagiarism, Academic integrity, Originality, Writing, Submission, Similarity report, Education, Checking, Citation, Academic misconduct, Integrity policies, Academic writing, Assessment",
            },
            {
                tags:"CamScanner, Scanning, Documents, Mobile, PDFs, Images, OCR, Storage, Share, Digitize, Notes, Capture, Edit, Organize",
            },
            {
                tags:"DALL-E, AI art, Image generation, Text-to-image, Creativity, OpenAI, Visuals, Artwork, Innovation, Machine learning, Generative model",
            },
            {
                tags:"Deep AI, Neural networks, Deep learning, Machine learning, Algorithms, Data, Training, Artificial intelligence, Models, Innovation, Research",
            },
            {
                tags:"exam,Coursera, Online courses, Education, Certificates, Specializations, MOOCs, Learning, Skill development, E-Learning, Universities, Instructors",
            },
            {
                tags:"Duolingo, Language, Learning, App, Courses, Gamification, Practice, Fluency, Vocabulary, Lessons, Mobile",
            },
            {
                tags:"Descript,audio, Video, Editing, Transcription, Collaboration, Multimedia, Podcasts, Projects, Scripting, Workflow, Creative",
            },
            {
                tags:"Brain.fm, Focus, Music, AI-generated, Productivity, Relaxation, Sleep, Cognitive enhancement, Soundscapes, Brainwave entrainment",
            },
            {
                tags:"Krisp, Noise cancellation,audio, Calls, Meetings, Productivity, Clarity, App, Remote work, Communication, Background noise",
            },
            {
                tags:"Replika, Chatbot, AI, Conversations, Personal growth, Mental health, Therapy, Emotional support, Text-based, Virtual friend",
            },
            
        ];
        const fuseOptions = {
            keys: ["tags"], // Specify the keys to search within
            threshold: 0.0, // Set threshold to 0 for exact word matching
        };

        // Create a new Fuse instance
        const fuse = new Fuse(data, fuseOptions);

        function filterTiles() {
            const searchInput = document.getElementById('searchInput').value.toLowerCase().trim();
            const tiles = document.querySelectorAll('.tile');

            tiles.forEach((tile, index) => {
                const tags = data[index].tags.split(',');
                const isMatch = tags.some(tag => searchInput.includes(tag));
                if (isMatch || searchInput === "") {
                    tile.style.display = 'block';
                } else {
                    tile.style.display = 'none';
                }
            });
        }

  