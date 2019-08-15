<script>
    import { Badge, Card } from 'sveltestrap';

    export let name = 'NAME';
    export let img;
    export let iniciative = 0;
    export let damage = 0;
</script>

<style>
  div.damage {
      background:red;
      color:white;
      padding:5px;
      float:left;
      width: 200px;
  }
</style>

<Card>
    <div>{name} - <Badge class="badge-success">{iniciative}</Badge></div>
    <div class="damage">Damage recieved: {damage}</div>
</Card>

