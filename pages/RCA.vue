<template>
    <section>
        <b-collapse class="card" animation="slide" aria-id="contentIdForA11y3">
            <div
                slot="trigger" 
                slot-scope="props"
                class="card-header"
                role="button"
                aria-controls="contentIdForA11y3">
                <p class="card-header-title">
                    Exclusions and Cautions for the use of RCA 
                </p>
                <a class="card-header-icon">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    <div class="columns">
                        <div class="column">
                            <h4>EXCLUSIONS</h4>

                            <ul>
                                <li> Liver Failure </li>
                                <li> Severe lactic acidosis</li>
                                <li> pH > 7.5 or HCO3 > 40 mmol/L</li>
                                <li> No central venous access  (exc. Vascath)</li>
                            </ul>
                        </div>
                        <div class="column">
                            <h4>CAUTIONS</h4>
                            <ul>
                                <li>Lactate >5 mmol/L</li>
                                <li>Chronic Liver disease</li>
                                <li>Post hepatic resection</li>
                            </ul>
                        </div>
                        
                    </div>
                </div>
            </div>
            <footer class="card-footer">
                <div class="card-footer-item">
                    <h1>Use only  Calcium-free dialysate  with 4mmol K+</h1>

                </div>
                
            </footer>
        </b-collapse>

        <br>
        

        <b-collapse class="card" animation="slide" aria-id="contentIdForA11y3">
            <div
                slot="trigger" 
                slot-scope="props"
                class="card-header"
                role="button"
                aria-controls="contentIdForA11y3">
                <p class="card-header-title">
                    Initial Calcium and pH check
                </p>
                <a class="card-header-icon">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    <ul>
                        <li>Check an [iCa] and pH on an ABG BEFORE starting CRRT</li>
                        <li>If [iCa] is <0.9 administer 10mL Calcium Gluconate (2.2mmol) infusion</li>
                        <li>Set the CALCIUM RATIO to start at 1.7 mmol/L of effluent</li>
                        <li>If re-starting the filter within 4 hours of disconnection, keep the previous ratio</li>
                        <li>Re-check Ca 30 min after starting and  any dose adjustments – titrate according to Ca table</li>
                    </ul>

                </div>
            </div>
            <!-- <footer class="card-footer">
                <a class="card-footer-item">Save</a>
                <a class="card-footer-item">Edit</a>
                <a class="card-footer-item">Delete</a>
            </footer> -->
        </b-collapse>
        <br>
        <b-collapse class="card" animation="slide" aria-id="contentIdForA11y3">
            <div
                slot="trigger" 
                slot-scope="props"
                class="card-header"
                role="button"
                aria-controls="contentIdForA11y3">
                <p class="card-header-title">
                    CITRATE and pH management – Initial setup 

                </p>
                <a class="card-header-icon">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    <ul>
                        <li>Use OMNISET-L or PRO sets only</li>
                        <li>PROGRAM Citrate ratio as 4 mmol/L of blood – NEVER ADJUST THIS RATIO</li>
                        <li>Set the CALCIUM RATIO to start at 1.7 mmol/L of effluent</li>
                        <li>Select initial and titration parameters according to the tables on the next page, depending on the patient’s IBW</li>
                        <li>If pH < 7.20 at the start  administer 50 mls  of 8.4% Bicarbonate over 30 min</li>
                        <li>Recheck pH and K+ 3-6 hourly and adjust according to tables</li>
                    </ul>

                </div>
            </div>
            <!-- <footer class="card-footer">
                <a class="card-footer-item">Save</a>
                <a class="card-footer-item">Edit</a>
                <a class="card-footer-item">Delete</a>
            </footer> -->
        </b-collapse>
        <br>

         <b-collapse class="card" animation="slide" aria-id="contentIdForA11y3">
            <div
                slot="trigger" 
                slot-scope="props"
                class="card-header"
                role="button"
                aria-controls="contentIdForA11y3">
                <p class="card-header-title">
                    CALCIUM MONITORING & ADJUSTMENT (During treatment)

                </p>
                <a class="card-header-icon">
                    <b-icon
                        :icon="props.open ? 'menu-down' : 'menu-up'">
                    </b-icon>
                </a>
            </div>
            <div class="card-content">
                <div class="content">
                    <Calcium />

                </div>
            </div>
            <!-- <footer class="card-footer">
                <a class="card-footer-item">Save</a>
                <a class="card-footer-item">Edit</a>
                <a class="card-footer-item">Delete</a>
            </footer> -->
        </b-collapse>


    </section>
</template>


             

