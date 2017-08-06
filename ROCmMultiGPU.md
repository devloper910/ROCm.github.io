



#### In-node			
[Large BAR support BAR = Base Address Register	Making the GPU memory visible BAR 1 Region 	Yes MI25,MI8, MI6]	(https://rocm.github.io/ROCmPCIeFeatures.html)
Base driver have P2P API support	This is done via ROCr (HSA) AGENT API with Peer to Peer support	Yes- Since ROCM version 1.0	(http://www.hsafoundation.com/html_spec111/HSA_Library.htm#Runtime/Topics/02_Core/hsa_iterate_agents.htm%3FTocPath%3DHSA%2520Runtime%2520Programmer%25E2%2580%2599s%2520Reference%2520Manual%2520Version%25201.1.1%2520%7CChapter%25202.%2520HSA%2520Core%2520Programming%2520Guide%7C2.3%2520System%2520and%2520agent%2520information%7C2.3.1%2520System%2520and%2520agent%2520information%2520API%7C_____18)
[HCC Language Runtime support of P2P	 ROCr Agent API	Yes- Since ROCM version 1.0](https://scchan.github.io/hcc/classhc_1_1accelerator.html#aebd49b998f9421bd032ea450cbafd247)
HIP Language Runtime support of P2P	P2P API's model after CUDA P2P API's 	Yes- Since ROCM version 1.0	http://rocm-developer-tools.github.io/HIP/group__PeerToPeer.html
OpenCL Language Runtime P2P API	Peer-to-Peer API  with Autocopy support over Intel QPI bus API name -  clEnqueueBufferCopyP2PAMD	ROCm 1.6.2 OpenCl  	
Communication Primitives Library	Helper Library to make it easier to use P2P  Via Communication Primitives	In Development	
IPC 	Inter Process Communication 	ROCm 1.4	
Out of Node			
Remote DMA technology  ( RDMA) 	Peer-to-Peer bridge driver for PeerDirect	YES -since ROCm 1.0	https://github.com/RadeonOpenCompute/ROCnRDMA
libibverbs	Linux RDMA library	YES -since ROCm 1.0	https://github.com/RadeonOpenCompute/ROCnRDMA
PeerDirect	Mellanox Peer API for Infiniband and	YES -since ROCm 1.0	https://community.mellanox.com/docs/DOC-2486
PeerDirectAsync	New Lighter Weight Peer access solution by Mellanox	In Development	http://downloads.openfabrics.org/WorkGroups/ofvwg/presentations/ofv_presentation_GPU.pdf
Standard Frameworks for Out of Node Communication			
OpenUCX	UCX is a communication library implementing high-performance messaging for MPI/PGAS frameworks	In Development	http://www.openucx.org. Source for ROCm https://github.com/openucx/ucx/tree/master/src/uct/rocm
OpenMPI	Open MPI Project is an open source Message Passing Interface https://www.open-mpi.org	In Development	https://github.com/openucx/ucx/wiki/OpenMPI-and-OpenSHMEM-installation-with-UCX
MPICH	MPICH is a high-performance and widely portable implementation of the Message Passing Interface (MPI) standard (MPI-1, MPI-2 and MPI-3) https://www.mpich.org/about/overview/	In Development	https://www.mpich.org/2016/08/30/mpich-3-3a1-released/  UCX support
OpenSHMEM	Partitioned Global Address Space & Communication Library	In Development	https://github.com/openucx/ucx/wiki/OpenMPI-and-OpenSHMEM-installation-with-UCX
[OSU benchmark to test performance](https://github.com/ROCm-Developer-Tools/OSU_Microbenchmarks)