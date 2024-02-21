# Demonstration

<!--
## Hrvatski centar kompentencija za HPC

[HR HPC CC](https://www.hpc-cc.hr/) uspostavljen je u sklopu projekta EuroCC (2020 - 2022) kao dio mreže nacionalnih centara kompetencija za HPC u 33 države članice Zajedničkog poduzeća za europsko računarstvo visokih performansi (EuroHPC JU).

One-Stop-Shop za HPC
- podrška korisnicima u korištenju HPC resursa
- razvoj novih kompetencija iz HPC područja
- suradnja akademske zajednice i gospodarstva
- izgradnja europskog HPC ekosustava

HR HPC CC trenutno djeluje u sklopu projekta EuroCC 2 (2023 - 2025) čiji je cilj daljnje promicanje korištenja HPC-a na nacionalnoj razini identificiranjem relevantnih korisnika.

```{figure} ../img/eurocc-map.png

```
-->

In this demonstration, we will show you the basic principle of how to access an HPC cluster, prepare a simple job and execute it on the compute nodes. The test system is the supercomputer [Supek](HPC-infra.md) operated by the University Computing Centre, University of Zagreb. The basic principles of work demonstrated in this course are similar on all other clusters and supercomputers, however, each might have its own software stack, hardware architecture and storage system.

The clusters your SSH protocol to access them.

The clusters use resource management and job submission systems - the compute nodes cannot be accessed directly by the user.


## A typical cluster workflow

```{callout} The basic steps are the following:
1. **Authenticatio**n (this step is done only once, at the first login).
   1. Generating SSH keys.
   2. Copy public key to the remove server.
2. **Connect to** remote server using secure shell protocol (SSH).
3. **Copy** your **data** using secure copy (e.g. scp, rsync).
4. **Prepare a script** that describe how your application and data will be executed.
5. **Allocate resources** and submit your job using job and resource management system (e.g. SLURM, PBS).
6. Once the job is finished, **retrieve output** data.
```

```{figure} ../img/demo-run.png
An example of a typical HPC workflow.
```
---
### Generate SSH keys

The first step is to authenticate the computer from which you plan to access the computer cluster. In this demo we will show to create SSH keys using command line. For more options check the Supek [documentation](https://wiki.srce.hr/pages/viewpage.action?pageId=121966392) (see 'Pristup klasteru Supek')

<link rel="stylesheet" type="text/css" href="../../_static/asciinema-player.css" />
<body>
  <div id="sshkey-gen"></div>
  ...
  <script src="../../_static/asciinema-player.min.js"></script>
  <script>
    AsciinemaPlayer.create('../../extra/keygen.cast', document.getElementById('sshkey-gen'), {
      loop: false,
      fit: "width",
      terminalFontSize: 'medium',
      cols: 100,
      rows: 30,
      markers: [8.85],
      pauseOnMarkers: true
      });
  </script>
</body>



### Upload public-key to Supek


### Loggin to login node

To log into to the Supek, we have to connect to the GPU login node: *login-gpu.hpc.srce.hr*.



Add figure Authentication -> Logging in -> Copying files -> Nodes and partitions -> Modules -> Running jobs with PBS (qsub) -> Running jobs with batch scripts (qsub)