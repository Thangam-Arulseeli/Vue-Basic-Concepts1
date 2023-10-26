    <template>

        <h5> My first VUE Component</h5>
        <hr  />
        {{title}} <br />
        Count value is : <strong> {{count}} </strong>
        <hr /> 

        <div class="text-secondary text-center">
            <p>My name is <u><b> {{firstName}}  {{lastName}} </b> </u> </p>
        </div>

        <div class="text-worning text-center">
          <h5> {{a}} * {{b}} = {{multiply() }}</h5>
            <br />
              Value  {{ a * 100 }}
            <br />
             Condition :   {{ status ? 'YES' : 'NO' }}
            <br />
            {{ title.split(' ').reverse().join(' ') }}
            <br />
         </div>
    </template>

  <script>
    export default {
        data() {
          return {  count: 100,
                    a: 10,
                    b: 20,
                    title : 'JS file with HTML file in VUE example',
                    status : true,
                    
                    firstName : "Arulseeli",
                    lastName : "Churchill"
            }
        },
        methods: 
        {
         multiply()
        {
          var c= this.a * this.b
          console.log(this.a + ' * ' + this.b + ' = ' + c )
          alert ('Hai!!!! ' + this.firstName + " " + this.lastName)
          return c
        }
        }
      }
    </script>