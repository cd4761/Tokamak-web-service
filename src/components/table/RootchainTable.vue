<template>
  <table class="rootchain-table">
    <thead>
      <tr>
        <th>Name</th>
        <th>Log</th>
        <th>Status</th>
        <th>*Status</th>
        <th>IP</th>
        <th>IP</th>
        <th>(re)set Scripts</th>
        <th>Is set?</th>
        <th>Start Node</th>
        <th>Deploy Seig Manager</th>
        <th>Deployed?</th>
        <th>Deploy PowerTON</th>
        <th>Deployed?</th>
        <th>Start PowerTON</th>
        <th>Started?</th>
        <th>Export Manager</th>
        <th>Exported?</th>
        <th>Created At</th>
        <th>Shutdown</th>
        <th>Drop</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(rootchain) in rootchainList" :key="rootchain" >
        <td><span class="pointer-name">{{ rootchain.name }}</span></td>
        <td>Log</td>
        <td>
          
          <input type="submit" name="Check" value="1.Check">
        </td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
      </tr>
    </tbody>
  </table>
</template>