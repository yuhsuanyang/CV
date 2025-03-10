<!--h1>Welcome to your library project</h1>
<p>Create your package using @sveltejs/package and preview/showcase your work with SvelteKit</p>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p-->
<script>
    import GeneralInfo from '$lib/components/GeneralInfo.svelte'
    import ExpSection from '$lib/components/ExpSection.svelte'
    import ProjectSection from '$lib/components/ProjectSection.svelte'
    import SkillSet from '$lib/components/SkillSet.svelte'
    import {PhoneSolid, MailBoxSolid} from 'flowbite-svelte-icons';
</script>
<div class="mx-1 my-4 font-serif text-sm">
    <div class="flex justify-center mx-8 my-4">
        <h1 class="text-3xl font-bold text-sky-700">Yu-Hsuan (Darcy) Yang</h1>
    </div>
    <div class="mx-8 flex items-center">
        <div class="flex gap-4">
            <div>
                <GeneralInfo icon="phone" info="(+886)953330882, (+65)88260500"/>
                <GeneralInfo icon="mail" info="sb0953330882@gmail.com"/>
            </div>
            <div>
                <GeneralInfo icon="github" info="https://github.com/yuhsuanyang"/>
                <GeneralInfo icon="linkedin" info="https://www.linkedin.com/in/yu-hsuan-yang-506a3b161/"/>
            </div>
        </div>
        <!--img src="/photo.jpeg" class="h-16"-->
    </div>
    <div class="mx-8">
        <div class="border-b-2 my-1 text-lg font-bold py-1 text-sky-600">Education</div>
        <ExpSection
             institute="Nanyang Technological University"
             location="Singapore"
             position="Master of Science in Financial Technology (Intelligent Process Automation Specialisation)"
             duration="Aug. 2024 - now"
             >
             <!--li>Track: Intelligent Process Automation Specialisation</li-->
             <div class="flex gap-4">
                 <li>Expect to graduate in June 2025</li>
                 <li>Trimester 1 GPA: 4.5/5</li>
             </div>
             <!--div class="flex gap-4">
                 <li>Coursework project: Portfolio Allocation with Reinforcement Learning (Did the RL algorithms from scartch and apply them to optimize the allocation between US bonds and emerging market stocks. The results beat the Min-Variance method.)
             </div-->
        </ExpSection>

        <ExpSection
             institute="National Chiao Tung University"
             location="Hsinchu, Taiwan"
             position="Master’s degree in Institute of Data Science and Engineering"
             duration="Sept. 2018 - June 2020"
             >
             <div class="flex gap-4">
                 <li>GPA: 3.91/4.3</li>
                <li>Dissertation: Dynamic Selection for Multivariate Time Series with Attention Networks</li>
             </div>
             <!--li>Capstone project: YouTube MV View Counts Forecasting</li-->
        </ExpSection>
        <ExpSection
             institute="National Cheng Kung University"
             location="Tainan, Taiwan"
             position="International Bachelor Degree Program on Energy"
             duration="Sept. 2014 - June 2018"
             >
             <div class="flex gap-4">
                 <li>Minor: Mathematics</li>
                 <li>GPA: 4.15/4.3</li>
                <li>Honors: 2014 Academic Achievement Award</li>
             </div>
        </ExpSection>
    </div>

    <div class="mx-8">
        <div class="border-b-2 text-lg font-bold my-1 py-1 text-sky-600">Work Experience</div>

        <ExpSection
            institute="RV Capital Management"
            location="Singapore"
            position="Intern Analyst"
            duration="Jan. 2025 - March 2025"
            >
            <li> This role implements LLM applications with LangChain to help with some business processes in the hedge fund company.
            <li>Automate financial document parsing task for the risk team by applying few-shot learning on LLM which reaches 90% accuracy and build Power BI dashboards on behalf of error analysis.</li>
            <li>Design a RAG-based chatbot that works with long documents by efficiently summarizing them and constructing vector databases.</li>
        </ExpSection>
        <ExpSection
            institute="Sinopac Holdings"
            location="Taipei, Taiwan"
            position="Assistant Manager, AI engineer in Digital Technology Division (DTD)"
            duration="Sept. 2020 - July 2024"
            >
            <li>Reinforcement learning in asset allocation: Aimed to maintain a portfolio of stocks that can beat the TWSE market based on their profile and transaction behaviors.</li>
            <li>Machine learning pipelines for customer analysis: Predicted the preferences of customers in certain financial products or campaigns based on their profile and transaction behaviors.</li>
            <li>Workload Orchestration: Optimized the utilization of computational resources in the development environment by k8s and docker. Currently working on single sign-on services.</li>
            <li>Risk and control self-assessment automation: Developed a pipeline to summarize the assessment advices from the risk control department by LLM, clustering and classification. </li>
            <li>Dojo for rapid AI demonstration: Designed a platform for displaying the GenAI and LLM applications developed by DTD. Responsible for the frontend development.</li>
        </ExpSection>
    </div>
    <div class="mx-8">
        <div class="border-b-2 text-lg font-bold my-1 py-1 text-sky-600">Extracurricular Certificates and Projects</div>
        <ProjectSection
            projectName="Dashboard to Dream Job: Career Success through Power BI Bootcamp"
            duration="March. 2025"
            >
            <li>Navigate Power BI interfaces, data integrgrity maintenance and conduct data modeling.</li>
            <li>Data preprocessing with DAX and optimize dashboards with other advanced visulization features. </li>

        </ProjectSection>
        <ProjectSection
            projectName="Big Data Workshop"
            duration="Nov. 2024"
            >
            <li>Learned about distribution computing system with GCP (Google Cloud Platform). Got hands-on experience of using Hadoop, Hive and Spark to perform data analyze.
  </li>
        </ProjectSection>
        <ProjectSection
            projectName="Bloomberg for Education"
            duration="Nov. 2024"
            >
            <li>Bloomberg Financial Fundamental: Gain knowledge of financial markets, risk and reward and porfolio management in the online courses.</li>
        </ProjectSection>
        <ExpSection
            institute="JPMorgan Chase & Co."
            location="www.theforage.com"
            position="Quantitative Research Virtual Experience Program"
            duration="Sept. 2024"
            >
            <li>Credit risk analyze: Converted FICO scores into categorical data with hyperopt and used decision tree to predict the customers' probability of default by loan data.</li>
            <li>Comodity storage contract price modeling: Use linear regression and cosine function to model both the periodicity and increment in natural gas data. Given injection, withdrawal and storage conditions (dates, rates, prices, cost, etc), calculated the value of the comodity contract.</li>
        </ExpSection>
    </div>

    <div class="mx-8">
        <div class="border-b-2 text-lg font-bold my-1 py-1 text-sky-600">Technical Skills</div>
        <div class="grid grid-cols-2 my-2">
            <SkillSet skillType="Programming" skills="C++, Python, SQL, Golang"/>
            <SkillSet skillType="AI & ML" skills="scikit-learn, Pytorch, LangChain"/>
            <SkillSet skillType="Finance" skills="Quantitative methods in risk and analysis"/>
            <SkillSet skillType="Web development" skills="HTML, CSS, Svelte, Django"/>
            <SkillSet skillType="Language proficiencies" skills="Mandarin(native), English(IELTS 7)"/>
        </div>
    </div>
</div>
