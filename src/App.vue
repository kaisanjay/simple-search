<script>
import { tutorials as tutorialData } from '../data'

export default {
  name: 'App',
  data: () => ({
    tutorials: []
  }),
  methods: {
    filterTutorials: function() {
        this.tutorials = tutorialData
    }
  },
  created: function() {
    this.filterTutorials()
  }

}
</script>

<style scoped>
  .container {
    max-width: 750px;
  }
  .footer {
    padding: 15px;
    color: #777;
    border-top: 1px solid #e5e5e5;
  }
  .header {
    margin: 10px 0 20px;
  }
</style>
