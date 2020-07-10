
<template>
 
    <div>
        <div class="field">
            <div class="control is-expanded">
                <div class="select is-rounded is-large is-success is-fullwidth">
                    <select :value="calcium.value" @change="onSelectChange($event, 'calcium')">
                        <option>calcium</option>
                        <option v-for="(item, calciumIndex) in calciumOptions" :key="calciumIndex" :data-index="calciumIndex" :value="item">{{item}}</option>
                    </select>
                
                </div>
            </div>
        </div>
        
            
        <div>
            Calcium Ratio (mmol/L):
            <p>{{CalciumRatio}}</p>
        </div>

       

        
        


    </div>
</template>
<script>
export default {
    data() {
        return {
            calcium: {
                index: 0,
                value: 'calcium'
            },
           

            calciumOptions: ['<0.8', '0.81-089','0.99','1.00-1.20','>1.20','>1.50'],
        
            values: 
            
                ["increase by 0.6","increase by 0.6","increase by 0.3 ", "No change recheck in 3 hours", "decrease by 0.3", "decrease by 0.6"]
                
               
            


            
        }
    },
    computed: {
        CalciumRatio() {
            try {
                if (Number.isInteger(this.calcium.index)) {
                    return this.values[this.calcium.index]
                    
                }
            } catch (error) {
                console.error(error)
            }

            return 'No value found'
        },

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