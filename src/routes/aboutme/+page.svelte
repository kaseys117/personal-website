<script lang="ts">
	import type { PageData } from './$types';

	let { data }: { data: PageData } = $props();
</script>

<h1>
	<center> About Me </center>
</h1>

<p class="text-center" style="color: #454863; margin-bottom: 2rem;">
	A couple of facts about me both professionally and personally.
</p>

<div class="aboutmebox">

		<div class="professional card">
			<h2>
				Professional Life
			</h2>

			<span>
				<strong>Job Experience</strong><br />
				&#10022; I'm currently working at Sam Houston State University as a System Analyst<br />
				<u>My Job Duties Include, but are Not Limited to</u><br />
				&#10022; Managing sensitive data, ensuring adherence to security standards and confidentiality
				requirements <br />
				&#10022; Utilizing Power BI for data analysis to track and report office statistics <br />
				&#10022; Optimizing office procedures by using automation <br />
				&#10022; Hardware and software auditing<br />
				&#10022; New system and hardware implementation<br /><br />
				<strong>Skills</strong><br />
				&#10022; Data analysis<br />
				&#10022; Network security monitoring<br />
				&#10022; Incident response<br />
				&#10022; Keen attention to detail<br />
				&#10022; Collaboration<br />
				<br />
				<strong>Tools</strong><br />
				&#10022; Power Automate<br />
				&#10022; Power BI<br />
				&#10022; Wireshark<br />
				&#10022; NMAP<br />
				&#10022; Metasploit<br />
			</span>
		</div>

		<div class="tools">
			<img src="Tools.png" style="width: 400px;" />
		</div>

		<div class="education card">
			<h2>Education</h2>

			<span>
				<strong>Degrees</strong><br />
				&#10022; Bachelor of Science in Cybersecurity - Sam Houston State University <br />
				&#10022; Associate of Science - Houston Community College <br /><br />
				<strong>Certifications</strong><br />
				&#10022; In August of 2023, I was accepted into the SANS Cyber Academy program <br />
				&#10022; After the completion of each course, I successfully earned 3 GIAC certifications; GFACT,
				GSEC, and GCIH <br /><br />
				<strong>Relevant Coursework</strong><br />
				&#10022; Malware analysis <br />
				&#10022; Network security <br />
				&#10022; Ethical hacking <br />
				&#10022; Digital forensics <br />
			</span>
		</div>

		<div class="logos">
			<img src="Logos.png" style="width: 400px;" />
		</div>

		<div class="personal card">
			<h2>
				Personal Life
			</h2>

			<span>
				<strong>Basics</strong><br />
				&#10022; Born and raised in Houston, TX <br />
				&#10022; Moved to Huntsville, TX in 2021 for college<br />
				&#10022; Studied cybersecurity at Sam Houston State, graduating with cum laude <br />
				&#10022; Married to my loving husband, Carlos<br />
				&#10022; Adopted a stray cat & named her Matcha<br />
				&#10022; Adopted another shelter kitten and named him Cornchip<br /><br />
				<strong>My Days Consist Of </strong><br />
				&#10022; Work<br />
				&#10022; Watching movies<br />
				&#10022; Going on walks<br />
				&#10022; Studying & working on cyber projects<br /><br />
				<strong>Lately I've Been Into</strong><br />
				&#10022; Teas<br />
				&#10022; Healthy lifestyles<br /> <br />
				<strong>I Aspire To Be</strong><br />
				&#10022; A cybersecurity expert (like Mr.Robot, but on the white hat side)<br>
				&#10022; A skilled piano player
				<!-- <br><br>If you'd like to know any further, I think it's time for some OSINT. -->
			</span>
		</div>

		<div class="photoboard">
			<img src="PhotoBoard.png" style="width: 400px;" alt="Photoboard with photos" />
		</div>

	<!-- <div class="futureprojects4">
    
            <div class="futureprojects">
    
                <h1 style="font-size: 26px; color: #454863; font-weight: normal; margin: 1px;"> Future Projects </h1>
    
    
            </div>
    
        </div> -->
</div>

<style>

.aboutmebox {
    display: grid;
    width: auto;
    gap: 2.5rem;
    margin: 0 2.5rem;
    grid-template-areas: 
    "professional tools"
    "education logos"
	"personal photoboard";
    align-items: center;
    grid-template-columns: 1fr auto;
}

.personal{
grid-area: personal;
}

.photoboard{
grid-area: photoboard;
}

.professional{
grid-area: professional;
}

.tools{
grid-area: tools;
}

.education{
grid-area: education;
}

.logos{
grid-area: logos;
}


.card{
    font-size: 16px;
    color: #454863;
    padding: 1.5rem 1.5rem 1rem 2rem;
    border: 1px solid white;
    border-radius: 1rem;
    box-shadow: 0px 4px 10px #d3cedb;
    background-color: #e5e2f4;
    width: 60ch;
    & span {
    display: block;
    margin: 1rem 0; 
    }    
}

h2{
font-size: 26px; color: #454863; font-weight: normal; margin: 1px;    
}

</style>