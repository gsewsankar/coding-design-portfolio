<svelte:head>
	<title>Garrick Sewsankar | Experience</title>
</svelte:head>

<script>

</script>

<style>
.experience{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
}

.job{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding-bottom: 50px;
}

.job .left{
    max-width: 500px;
}

img{
    width: auto;
    height: 200px;
}


@media only screen and (max-width: 600px) {
.experience{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
}

.job{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-bottom: 50px;
}

.job .left{
    max-width: 300px;
}

img{
    width: auto;
    height: 100px;
}
	
}
</style>

<h1> Experience </h1>

<div class="experience" id="experience">
    <div class="job">
        <div class="left">
            <h2>Full Stack Developer</h2>
            <div><b>fwee</b> Orlando, FL <b>4/2021-Present</b></div>
            <p>
                <a href="https://fwee.io" target="_blank" rel="noopener noreferrer"><b>fwee.io</b></a><br> 
                Responsible for the system design and maintenance of a scalable social platform that utilizes Google cloud functions within a virtual marketplace.
                Built and designed a client with React to display user information retrieved from an API that I developed with GraphQL to handle accounting data and transactions for each user’s account. 
            </p>
        </div>
        <div class="right">
            <img src=fwee_logo.svg alt=brkn/>
            <img src=fweemobile.png alt="brkn"/>
        </div>
    </div>

    <div class="job">
        <div class="left">
            <h2>E1 Technician</h2>
            <div><b>PHILIPS (Invivo)</b> Gainesville, FL <b>12/2019-12/2020</b></div>
            <p>
                Assembled and tuned MRI Radiofrequency coils by soldering components to boards and calibrating the coils to work with correct frequencies.
                Completed documentation for each coil built and met manufacturing production deadlines each week.
            </p>
        </div>
        <div class="right">
            <img src=https://cdn.freelogovectors.net/wp-content/uploads/2018/04/philips_logo.png alt=brkn/>
            <img src="https://images.philips.com/is/image/PhilipsConsumer/HCNMRB209-IMS-en_US?wid=470&$pnglarge$" alt="brkn"/>
        </div>
    </div>

    <div class="job">
        <div class="left">
            <h2>Undergraduate Researcher</h2> 
            <div><b>UF Transportation Institute & JainLab</b> Gainesville, FL <b>10/2018-6/2019</b></div>  
            <p>
                Analyzed video eye tracking data by creating regions of interest using
                BeGaze software on a driving safety project under the I-STREET initiative.
                Research was used to determine where drivers look while driving and if
                audio alerts would help protect pedestrians and cyclists.
            </p>
        </div>
        <div class="right">
            <img src="https://fdotwww.blob.core.windows.net/sitefinity/images/default-source/content1/info/logo/png/fdot_logo_color.png?sfvrsn=293c15a8_2" alt=brkn/>
            <img src="https://www.transportation.institute.ufl.edu/wp-content/uploads/2019/05/I-STREET-Logo-400px-300x233.png" alt="brkn"/>
        </div>
    </div>
      
</div>