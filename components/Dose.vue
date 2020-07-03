
<template>
 
    <div>
        <div class="select is-rounded is-large is-success">
            <select :value="ph.value" @change="onSelectChange($event, 'ph')">
                <option>pH</option>
                <option v-for="(item, phIndex) in phOptions" :key="phIndex" :data-index="phIndex" :value="item">{{item}}</option>
            </select>
        </div>
         <div class="select is-rounded is-large is-success ">
            <select :value="potassium.value" @change="onSelectChange($event, 'potassium')">
                <option>K+</option>
                <option v-for="(item, potassiumIndex) in potassiumOptions" :data-index="potassiumIndex" :key="potassiumIndex">{{item}}</option>
            </select>
        </div>
        <div>
            Dialysate Flow Rate (QD):
            <p>{{dialysateFlowrateValue}}</p>
        </div>

         <div>
            Blood Flow (QB):
            <p>{{bloodFlowrateValue}}</p>
        
        </div>

        
        


    </div>
</template>
<script>
export default {
    data() {
        return {
            ph: {
                index: 0,
                value: 'pH'
            },
            potassium: {
                index: 0,
                value: 'K+'
            },

            phOptions: ['<7.10', '7.10-7.19','7.20-7.29','7.30-7.39','7.40-7.44','7.45-7.49','7.50-7.54', '>7.55'],
            potassiumOptions: [">6.0","5.6-6.0","5.1-5.5", "4.6-5.0", "4.0-4.5", "<4.0"],
            values: [
                ["2300","2100","1900", "1800", "1600", "1400"],
                ["2300","2100","1900", "1700", "1500", "1400"],
                ["2200","2100","1900", "1700", "1400", "1400"],
                ["2200","2000","1800", "1600", "1400", "1400"],
                ["2200","1900","1700", "1500", "1400", "1400"],
                ["2300","2100","1900", "1900", "1700", "1700"],
                ["STOP","2300","2100", "2100", "2100", "2100"],
                ["STOP","STOP","STOP","STOP","STOP","STOP"]
            ],

            blood: [
                '130','120','110','100','80','80','80','STOP'
                
            ],
            
        }
    },
    computed: {
        dialysateFlowrateValue() {
            try {
                if (Number.isInteger(this.ph.index) && Number.isInteger(this.potassium.index)) {
                    return this.values[this.ph.index][this.potassium.index]
                    
                }
            } catch (error) {
                console.error(error)
            }

            return 'No value found'
        },

        bloodFlowrateValue() {
            try {
                if (Number.isInteger(this.ph.index) && Number.isInteger(this.potassium.index)) {
                    return this.blood[this.ph.index]
                    
                }
            } catch (error) {
                console.error(error)
            }

            return 'No value found'
        }


       
            
        
    },
    methods: {
        onSelectChange(e, key) {
            const value = e.target.value
            const index = this[`${key}Options`].findIndex(item => item == value)
            this[key] = {
                index,
                value
            }
        }
    }
}
</script>
<style lang="scss" scoped>

</style>

