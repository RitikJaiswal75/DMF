# Previewing
    The preview process may be considered to carry a significant risk of violating the ACPO’s first principle, because it requires direct examination of the suspect devices.
### Offline preview
    In a typical preview situation, the device to be previewed will be dealt with in an offline state.

    i.e, it will have been disconnected from networks and shut down to allow the examiner to remove storage devices for connection to a trusted preview workstation.

    Ideally, devices will be connected through a write-blocking device to ensure that ACPO Principle 1 is still upheld.

    it is possible to use a common USB write-blocker to protect them against accidental digital contamination.
### Online Preview
    The major disadvantage of offline preview is the requirement to shut down the device under examination and gain physical access to the storage devices it contains.

    The preview examination will be carried out on a live system, which is undergoing changes of state and which cannot be considered to be completely trustworthy.

    Programs such as rootkits, which are designed to implant themselves into a system to allow an attacker to abuse that system
    In order to conduct an online preview, most examiners have access to trusted tools on read-only media such as CDs.

    These tools have been written in a trusted environment and the CD contains all the code necessary to allow them to run without using any code from the suspect system

    They tend, also, to be written in such a way that they protect the suspect system from accidental changes to data, apart from the necessary changes to primary RAM to run the trusted tools themselves
# Continuity and hashing
    At the highest level, one or more hash values will be computed for the data on the original device.

    Because the image has been produced from this device, and contains identical data, the hash value for the image should match, exactly.

    Original Hashing algorithms such as MD5, SHA-1 and SNEFRU are very sensitive to changes in data, and the modification of even a single bit
# Imaging
    To produce an accurate copy of a digital storage device, we need to use a method which will produce a complete copy of the device, including all unused space, deleted data and, if possible, damaged areas.
### Offline Imaging
    In this process, the suspect device is connected to an imaging workstation using a write-blocker.

    The imaging software is then used to read data from the device and store it to either a file or separate device.

    Once imaging is complete, the first copy is usually considered to be the master copy and further working copies can be generated as required
### Online Imaging
    The storage device is left in situ and live imaging tools are used to capture data from it using the accompanying hardware.

    Of course, this poses similar problems to online previewing, but the use of trusted tools goes some way to mitigating these.

    The trusted tools allow the examiner to copy the device to either an external storage device, such as a USB hard disc, or across a network to a dedicated storage server

# Seven Element Security Model
<img src="./Picture1.png" />
    It contains seven key elements which are inter-linked to compose the system as a whole.

    Each of these elements must be secure in its own right and depends on its neighboring elements to ensure this.

    If there is a weakness in any one of the elements, the whole system is insecure and may be attacked/abused through the weak element(s).
### Entities
    Entities are objects which can manipulate and/or be manipulated by the system, and may be passive or active.
    
    Passive entities are external to the system, and are represented by collections of data which the system processes in some way. 

    Active entities tend to be part of the system and are responsible for choosing and controlling which processing should be performed. 
### Environment
    The environment represents the set of constraints or restrictions imposed on entities in an attempt to make them behave correctly. 
### Organization
    The organization contains the framework which allows those restraints and controls to be created, enforced and inter-related to each other while still allowing entities to co-operate and collaborate as necessary. 
### Infrastructure
    Infrastructure is the supporting mechanism required to enable activities within the organization. It is generally composed of physical components
### Activities
    Activities are complete tasks, often representing a complete transaction, from end to end. Activities can be single procedures but may be composites made up of multiple procedures. 
    
    Insecure activities are those which are poorly defined or understood and which have the potential to allow unwanted side-effects to occur. 
### Procedures
    At the procedure level, we are considering single tasks which represent discrete, identifiable, atomic (indivisible) processes within the wider context of an activity. 

    By breaking them down into procedures which can be described simply and quickly, we increase the chances of identifying any activity that are weakly defined or more likely to result in unwanted or unexpected results 
### Data
    The representation of the entities which the system is concerned with manipulating. Two key areas of security apply to data. 

    Firstly, the system must have a mechanism to ensure that data integrity is maintained, i.e. there must be a way to make sure that all data held are accurate and can be maintained correctly. 
    
    Secondly, the data must be protected from accidental damage or leakage 
    
    Because data represents something about entities, such as details of bank accounts, it is often seen as the direct target of an attack. 
    
    Any failings in data security, through flawed procedures, activities, infrastructure, organization, environment or entities, leaves the system vulnerable. 
