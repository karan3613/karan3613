<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Profile - The Ninja Way</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: '🦊';
            position: absolute;
            font-size: 200px;
            opacity: 0.1;
            top: -50px;
            right: -50px;
        }
        
        .header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .header .tagline {
            font-size: 1.3em;
            font-weight: 300;
        }
        
        .content {
            padding: 40px;
        }
        
        .section {
            margin-bottom: 50px;
        }
        
        .section-title {
            font-size: 2em;
            color: #667eea;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid #f093fb;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .jutsu-card {
            background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%);
            border-left: 5px solid #667eea;
            padding: 25px;
            margin: 20px 0;
            border-radius: 10px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .jutsu-card:hover {
            transform: translateX(10px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.3);
        }
        
        .jutsu-header {
            font-size: 1.5em;
            color: #f5576c;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .jutsu-subtitle {
            font-style: italic;
            color: #666;
            margin-bottom: 15px;
        }
        
        .skill-list {
            list-style: none;
            padding-left: 0;
        }
        
        .skill-list li {
            padding: 8px 0;
            padding-left: 30px;
            position: relative;
        }
        
        .skill-list li::before {
            content: '⚡';
            position: absolute;
            left: 0;
        }
        
        .code-block {
            background: #2d2d2d;
            color: #f8f8f2;
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            overflow-x: auto;
            font-family: 'Courier New', monospace;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .code-comment {
            color: #6272a4;
        }
        
        .code-keyword {
            color: #ff79c6;
        }
        
        .code-string {
            color: #f1fa8c;
        }
        
        .achievement-badge {
            display: inline-block;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            margin: 5px;
            font-weight: bold;
        }
        
        .quote-box {
            background: #fff9e6;
            border-left: 5px solid #ffd700;
            padding: 20px;
            margin: 20px 0;
            font-style: italic;
            border-radius: 5px;
        }
        
        .mission-table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .mission-table th {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px;
            text-align: left;
        }
        
        .mission-table td {
            padding: 15px;
            border-bottom: 1px solid #eee;
        }
        
        .mission-table tr:hover {
            background: #f5f5f5;
        }
        
        .cta-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px;
            text-align: center;
            border-radius: 15px;
            margin: 30px 0;
        }
        
        .cta-section h2 {
            margin-bottom: 20px;
        }
        
        .highlight {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 2px 8px;
            border-radius: 5px;
            font-weight: bold;
        }
        
        .emoji-large {
            font-size: 2em;
        }
        
        @media (max-width: 768px) {
            .header h1 {
                font-size: 2em;
            }
            
            .content {
                padding: 20px;
            }
            
            .jutsu-card:hover {
                transform: none;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🍜 The Developer Who Never Gives Up</h1>
            <p class="tagline">Believe it! I'm gonna be the greatest full-stack engineer!</p>
        </div>
        
        <div class="content">
            <div class="section">
                <p style="font-size: 1.2em; color: #666; margin-bottom: 30px;">
                    Yeah, I said it. While others were choosing between frontend or backend, mobile or AI, I decided to master them ALL. They said it was impossible. They said pick one path. But that's never been my ninja way.
                </p>
                <p style="font-size: 1.2em; color: #666;">
                    I'm the developer who turns impossible projects into shipped products. The one who brings AI, mobile, and backend together like a perfect team jutsu. And just like Naruto, I never back down from a challenge.
                </p>
            </div>

            <div class="section">
                <h2 class="section-title"><span class="emoji-large">🦊</span> My Ninja Arsenal: Three Powerful Jutsu</h2>
                
                <div class="code-block">
<span class="code-comment">// Inside every great developer is a chakra system of skills</span>
<span class="code-keyword">class</span> Uzumaki_Dev {
    constructor() {
        <span class="code-comment">// Three powerful forces, each a complete fighting style</span>
        this.jutsuArsenal = {
            rasengan: <span class="code-string">"Native Mobile Development"</span>,    <span class="code-comment">// Speed & Precision</span>
            shadowClone: <span class="code-string">"AI & Deep Learning"</span>,        <span class="code-comment">// Raw Intelligence</span>
            sageMode: <span class="code-string">"Scalable Backend Systems"</span>      <span class="code-comment">// Unlimited Stamina</span>
        };
    }
    
    unleashPower(challenge) {
        <span class="code-comment">// Can fight with one jutsu or unleash all three</span>
        <span class="code-comment">// Either way, the mission gets completed!</span>
        <span class="code-keyword">return</span> this.jutsuArsenal.transform(challenge);
    }
}

<span class="code-comment">// Dattebayo! 🍥</span>
                </div>
            </div>

            <div class="section">
                <div class="jutsu-card">
                    <h3 class="jutsu-header">📱 Rasengan Style: Native Mobile Development</h3>
                    <p class="jutsu-subtitle">My signature move—perfected through countless hours of training!</p>
                    <p style="margin-bottom: 15px;">
                        Just like Naruto spent years perfecting the Rasengan, I've mastered native mobile development. When I create apps, they're as smooth and powerful as a perfectly formed Rasengan spinning in your hand:
                    </p>
                    <ul class="skill-list">
                        <li><strong>iOS Mastery:</strong> Swift & SwiftUI—apps that make users go "Believe it!"</li>
                        <li><strong>Android Power:</strong> Kotlin (Jetpack Compose) & Java (XML)—native jutsu, no clones</li>
                        <li><strong>Perfect Form UX:</strong> Every screen, every interaction crafted with precision</li>
                        <li><strong>Lightning Speed Performance:</strong> 60fps animations, optimized chakra (battery), perfect flow</li>
                        <li><strong>Summoning Jutsu Architecture:</strong> MVVM, Clean patterns that scale like Gamabunta</li>
                    </ul>
                    <p style="margin-top: 15px; color: #f5576c; font-weight: bold;">
                        ⭐ This is my strongest technique. No shortcuts, no hybrid compromises—just pure, powerful, native experiences.
                    </p>
                </div>

                <div class="jutsu-card">
                    <h3 class="jutsu-header">🧠 Shadow Clone Jutsu: AI & Deep Learning</h3>
                    <p class="jutsu-subtitle">Create intelligent systems that work while you sleep!</p>
                    <p style="margin-bottom: 15px;">
                        Like Naruto's Shadow Clones that can learn and work independently, my AI systems operate autonomously and intelligently:
                    </p>
                    <ul class="skill-list">
                        <li><strong>Neural Network Training:</strong> PyTorch/TensorFlow—turning data into wisdom like a Sage</li>
                        <li><strong>Autonomous AI Agents:</strong> Systems that reason, plan, and execute independently</li>
                        <li><strong>Generative AI Summoning:</strong> LLMs and diffusion models at my command</li>
                        <li><strong>Chakra Control Foundation:</strong> DSA & Core Java—the basics done right</li>
                        <li><strong>Full Deployment Path:</strong> End-to-end ML that hits production with impact</li>
                    </ul>
                    <p style="margin-top: 15px; color: #f5576c; font-weight: bold;">
                        💡 I build AI that doesn't just look cool in demos—it protects the village (solves real problems)!
                    </p>
                </div>

                <div class="jutsu-card">
                    <h3 class="jutsu-header">🏗️ Sage Mode: Scalable Backend Engineering</h3>
                    <p class="jutsu-subtitle">Unlimited stamina—servers that never give up, never break down!</p>
                    <p style="margin-bottom: 15px;">
                        In Sage Mode, Naruto's chakra becomes unlimited and his senses sharpen. My backends operate the same way—infinite scale with perfect awareness:
                    </p>
                    <ul class="skill-list">
                        <li><strong>Multi-Clone APIs:</strong> RESTful and GraphQL systems that multiply to handle any load</li>
                        <li><strong>Summoning Technique Databases:</strong> SQL and NoSQL—right summon for every battle</li>
                        <li><strong>Barrier Ninjutsu Cloud:</strong> Auto-scaling, self-healing, always protecting</li>
                        <li><strong>Sealing Jutsu Security:</strong> Lock down data tighter than the Nine-Tails was sealed</li>
                        <li><strong>Perfect Optimization:</strong> Caching, load balancing—efficiency at maximum level</li>
                    </ul>
                    <p style="margin-top: 15px; color: #f5576c; font-weight: bold;">
                        🔥 When traffic hits like a Tailed Beast Ball, my backend tanks it without breaking a sweat!
                    </p>
                </div>

                <div class="jutsu-card" style="background: linear-gradient(135deg, #ffd70020 0%, #ff8c0020 100%); border-left: 5px solid #ffd700;">
                    <h3 class="jutsu-header" style="color: #ff8c00;">🦊 Nine-Tails Chakra Mode: Full-Stack Fusion</h3>
                    <p class="jutsu-subtitle">When I combine all three powers—that's when I'm unstoppable!</p>
                    <p style="margin-bottom: 15px;">
                        Most developers can't handle this much power. But like Naruto mastering Kurama, I've learned to unite all my abilities:
                    </p>
                    <ul class="skill-list">
                        <li><strong>Kurama Link Mode:</strong> On-device AI (CoreML, TensorFlow Lite) running at chakra speed</li>
                        <li><strong>Perfect Synchronization:</strong> Real-time ML pipelines from backend to mobile</li>
                        <li><strong>Bijuu Mode Apps:</strong> Native experiences powered by intelligent infrastructure</li>
                        <li><strong>Six Paths Power:</strong> Performance optimization that feels like you've been blessed</li>
                    </ul>
                    <p style="margin-top: 15px; color: #ff8c00; font-weight: bold;">
                        ⚡ This is my ultimate form—where mobile, AI, and backend work together like Team 7 at their peak!
                    </p>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title"><span class="emoji-large">🏆</span> Chunin Exams Passed: Battle-Tested</h2>
                <p style="margin-bottom: 20px;">
                    <span class="achievement-badge">3× Hackathon Champion</span>
                    <span class="achievement-badge">Multiple Top Finishes</span>
                    <span class="achievement-badge">Jonin-Level Execution</span>
                </p>
                <p style="font-size: 1.1em; margin-bottom: 15px;">
                    Hackathons are my Chunin Exams—where I prove I'm ready for bigger missions:
                </p>
                <ul class="skill-list">
                    <li><strong>24-Hour Forest of Death:</strong> Build and deploy in impossible timeframes</li>
                    <li><strong>Preliminary Matches:</strong> Mobile? AI? Backend? I can solo any challenge</li>
                    <li><strong>Final Tournament:</strong> Clutch execution when everyone's watching</li>
                    <li><strong>Talk-no-Jutsu:</strong> Convince judges why my solution is the one to believe in</li>
                </ul>
            </div>

            <div class="section">
                <h2 class="section-title"><span class="emoji-large">💭</span> My Ninja Way (This Is My Promise)</h2>
                <div class="quote-box">
                    <p style="font-size: 1.2em; margin-bottom: 15px;">
                        <strong>"I'm not gonna run away, I never go back on my word! That's my nindo, my ninja way—and it applies to code too."</strong>
                    </p>
                    <p style="margin-bottom: 10px;">✊ I won't half-ass mobile development.</p>
                    <p style="margin-bottom: 10px;">✊ I won't ship AI that doesn't work.</p>
                    <p style="margin-bottom: 10px;">✊ I won't build backends that crash under load.</p>
                    <p style="margin-top: 15px; font-size: 1.1em;">
                        When I commit to a project, I see it through to the end. When I write code, it ships, it scales, and it works. <strong>Because that's MY developer way!</strong>
                    </p>
                </div>
            </div>

            <div class="section">
                <h2 class="section-title"><span class="emoji-large">⚔️</span> Mission Board: Pick Your Rank</h2>
                <table class="mission-table">
                    <thead>
                        <tr>
                            <th>Mission Difficulty</th>
                            <th>Required Ninja Technique</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td><strong>A-Rank:</strong> "Need pixel-perfect native iOS/Android"</td>
                            <td>📱 Rasengan Style (my specialty)</td>
                        </tr>
                        <tr>
                            <td><strong>A-Rank:</strong> "Need custom ML models trained"</td>
                            <td>🧠 Shadow Clone Jutsu (AI mastery)</td>
                        </tr>
                        <tr>
                            <td><strong>A-Rank:</strong> "Backend can't handle our growth"</td>
                            <td>🏗️ Sage Mode (infrastructure)</td>
                        </tr>
                        <tr>
                            <td><strong>S-Rank:</strong> "Need full-stack ownership"</td>
                            <td>🦊 Nine-Tails Chakra Mode (complete mastery)</td>
                        </tr>
                        <tr>
                            <td><strong>S-Rank:</strong> "Emergency—ship now!"</td>
                            <td>🔥 All techniques, Baryon Mode activated</td>
                        </tr>
                    </tbody>
                </table>
            </div>

            <div class="cta-section">
                <h2>🤝 Join My Team (Let's Form Squad 7)</h2>
                <p style="font-size: 1.2em; margin: 20px 0;">
                    Whether you need refined mobile experiences, battle-tested AI, unbreakable infrastructure, or a ninja who can handle all three—<span class="highlight">I'm your guy. Believe it!</span>
                </p>
                <p style="margin-top: 30px; font-size: 1.1em;">
                    📬 <strong>Send a Messenger Hawk</strong><br>
                    Got an S-Rank mission? Ambitious village to protect? Just want to grab some ramen and talk tech?
                </p>
            </div>

            <div style="text-align: center; padding: 30px; background: #f9f9f9; border-radius: 15px; margin-top: 30px;">
                <p style="font-style: italic; color: #666; margin-bottom: 15px;">
                    <em>P.S. — If you read this whole thing, you're definitely someone who appreciates developers with determination and range. The kind of teammate who'd have my back in any fight.</em>
                </p>
                <p style="font-size: 1.3em; color: #f5576c; font-weight: bold;">
                    "I'm not gonna run away and I never go back on my word—that's my developer nindo!" 🦊🔥
                </p>
                <p style="margin-top: 15px; color: #999; font-size: 0.9em;">
                    — A developer who believes every project deserves a hero who never gives up
                </p>
            </div>
        </div>
    </div>
</body>
</html>
## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/https://www.linkedin.com/in/karan-chouhan-57a337283/) [![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/@https://www.youtube.com/@Z4TCH3) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:karanchouhan.3613@gmail.com) 

# 💻 Tech Stack:
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![GraphQL](https://img.shields.io/badge/-GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white) ![Kotlin](https://img.shields.io/badge/kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white) ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white) ![PowerShell](https://img.shields.io/badge/PowerShell-%235391FE.svg?style=for-the-badge&logo=powershell&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Swift](https://img.shields.io/badge/swift-F54A2A?style=for-the-badge&logo=swift&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase) ![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white) ![Netlify](https://img.shields.io/badge/netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=#00C7B7) ![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white) ![Heroku](https://img.shields.io/badge/heroku-%23430098.svg?style=for-the-badge&logo=heroku&logoColor=white) ![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka) ![Apache Hadoop](https://img.shields.io/badge/Apache%20Hadoop-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black) ![nVIDIA](https://img.shields.io/badge/cuda-000000.svg?style=for-the-badge&logo=nVIDIA&logoColor=green) ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi) ![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white) ![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white) ![OpenGL](https://img.shields.io/badge/OpenGL-%23FFFFFF.svg?style=for-the-badge&logo=opengl) ![Qt](https://img.shields.io/badge/Qt-%23217346.svg?style=for-the-badge&logo=Qt&logoColor=white) ![RabbitMQ](https://img.shields.io/badge/rabbitmq-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white) ![Apache Tomcat](https://img.shields.io/badge/apache%20tomcat-%23F8DC75.svg?style=for-the-badge&logo=apache-tomcat&logoColor=black) ![Apache](https://img.shields.io/badge/apache-%23D42029.svg?style=for-the-badge&logo=apache&logoColor=white) ![AmazonDynamoDB](https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?style=for-the-badge&logo=Amazon%20DynamoDB&logoColor=white) ![Firebase](https://img.shields.io/badge/firebase-a08021?style=for-the-badge&logo=firebase&logoColor=ffcd34) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Scipy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![GitLab](https://img.shields.io/badge/gitlab-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white) ![GitLab CI](https://img.shields.io/badge/gitlab%20CI-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white) ![FFmpeg](https://shields.io/badge/FFmpeg-%23171717.svg?logo=ffmpeg&style=for-the-badge&labelColor=171717&logoColor=5cb85c) ![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=for-the-badge&logo=Raspberry-Pi) ![nVIDIA](https://img.shields.io/badge/nVIDIA-%2376B900.svg?style=for-the-badge&logo=nVIDIA&logoColor=white) ![Unreal Engine](https://img.shields.io/badge/unrealengine-%23313131.svg?style=for-the-badge&logo=unrealengine&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=karan3613&theme=dark&hide_border=false&include_all_commits=true&count_private=true)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=karan3613&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=karan3613&theme=dark&hide_border=false&include_all_commits=true&count_private=true&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=karan3613&theme=radical&no-frame=false&no-bg=true&margin-w=4)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

  ## 💰 You can help me by Donating
  [![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/https://buymeacoffee.com/karan3613) 

  
<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
