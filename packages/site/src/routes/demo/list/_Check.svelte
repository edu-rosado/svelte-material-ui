<div>
  <List class="demo-list" checkList>
    <Item>
      <Label>Bruce Willis</Label>
      <Meta>
        <Checkbox bind:group={selected} value="Bruce Willis" />
      </Meta>
    </Item>
    <Item>
      <Label>Tom Hanks</Label>
      <Meta>
        <Checkbox bind:group={selected} value="Tom Hanks" />
      </Meta>
    </Item>
    <Item>
      <Label>Jack Nicholson</Label>
      <Meta>
        <Checkbox bind:group={selected} value="Jack Nicholson" />
      </Meta>
    </Item>
    <Item>
      <Label>Leonardo DiCaprio</Label>
      <Meta>
        <Checkbox bind:group={selected} value="Leonardo DiCaprio" />
      </Meta>
    </Item>
    <Item>
      <Label>Matt Damon</Label>
      <Meta>
        <Checkbox bind:group={selected} value="Matt Damon" />
      </Meta>
    </Item>
  </List>
</div>

<pre class="status">Selected: {selected.join(', ')}</pre>

<script lang="ts">
  import List, { Item, Meta, Label } from '@smui/list';
  import Checkbox from '@smui/checkbox';

  let selected = ['Tom Hanks'];
</script>

<style>
  * :global(.demo-list) {
    max-width: 300px;
  }
</style>
