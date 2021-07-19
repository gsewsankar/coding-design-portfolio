<svelte:head>
	<title>Garrick Sewsankar | Experience</title>
</svelte:head>

<script>

</script>

<style>
.experience
{
	margin: 1rem;
	display: flex;
	flex-direction: column;
}

.internships 
{
    display: flex;
    flex-direction: column;
}

.internship-location 
{
    padding-left: 1rem;
    display: flex;
    justify-content: space-between;
    font-size: 22px;
    color: rgb(95, 95, 95);
}

.internship-position 
{
    padding-left: 1rem;
    display: flex;
    justify-content: space-between;
    font-size: 18px;
    color: black;
}

.internship-description 
{
    padding-left: 3rem;
    display: flex;
    flex-direction: column;
}

.images{
    display: flex;
    flex-direction: row;
}

@media only screen and (max-width: 600px) {
	
}
</style>

<h1> Experience </h1>

<div class="experience" id="experience">
  <div class="internships">
      <div class="internship-location"> <b>PHILIPS</b> <div> Gainesville, FL </div></div>
      <div class="internship-position"> E1 Technician <div> December 2019 - December 2020 </div></div>
      <div class="internship-description"> 
          <ul>
              <li>Assembled and tuned MRI Radiofrequency coils by soldering components to boards and calibrating the coils to work with correct frequencies. </li>
              <li>Completed documentation for each coil built and met manufacturing production deadlines each week.</li>
          </ul>
      </div>
      <div class="images">
        <img width=200px height="auto" src="https://images.philips.com/is/image/PhilipsConsumer/HCNMRB209-IMS-en_US?wid=470&$pnglarge$" alt="brkn"/>
        <img width=100px height="auto" src=https://cdn.freelogovectors.net/wp-content/uploads/2018/04/philips_logo.png alt=brkn/>
      </div>
      <p></p>
      <div class="internship-location"> <b>UF Transportation Institute & JainLab</b> <div> Gainesville, FL </div></div>
      <div class="internship-position"> Undergraduate Researcher <div> October 2018 - June 2019 </div></div>
      <div class="internship-description"> 
          <ul>
              <li>
                  Analyzed video eye tracking data by creating regions of interest using
                  BeGaze software on a driving safety project under the I-STREET initiative.
              </li>
              <li>
                  Research was used to determine where drivers look while driving and if
                  audio alerts would help protect pedestrians and cyclists.
              </li>
          </ul>
      </div>
      <p></p>
  </div>
</div>