---
uid: General_Main_Release_10.6.0_changes
---

# General Main Release 10.6.0 – Changes (preview)

> [!IMPORTANT]
> We are still working on this release. Some release notes may still be modified or moved to a later release. Check back soon for updates!

## Changes

### Enhancements

#### DataMiner installer has been updated [ID 40409] [ID 41299]

<!-- MR 10.6.0 - FR 10.5.1 -->

The DataMiner installer has been updated.

When the configuration window appears, it will now be possible to either continue with the configuration or cancel the entire installation.

For more information on the installer, see [Installing DataMiner using the DataMiner Installer](xref:Installing_DM_using_the_DM_installer).

#### Service & Resource Management: Process of starting blocking tasks has now been optimized [ID 41175]

<!-- MR 10.6.0 - FR 10.5.1 -->

Up to now, when blocking tasks with the same start time needed to be scheduled for several bookings, in some cases, bookings with limited start actions could get blocked by bookings with longer start actions.

Because of a number of enhancements, the process of starting blocking tasks has now been optimized.

#### Service & Resource Management: Enhanced deletion of ReservationInstances in bulk [ID 41236]

<!-- MR 10.6.0 - FR 10.5.1 -->

When ReservationInstances were deleted in bulk, up to now, an individual delete request would be sent to the database for every instance.

From now on, when ReservationInstances are deleted in bulk, a single delete request will be sent to the database for every batch of 200 ReservationInstances.

This will significantly enhance overall performance when deleting large numbers of ReservationInstances.

#### SLAnalytics: Synchronization of the configuration.xml file can now be forced via Cube [ID 41270]

<!-- MR 10.6.0 - FR 10.5.1 -->

Up to now, when you had made changes to a *C:\\Skyline DataMiner\\Analytics\\configuration.xml* file on the leader Agent, you had to manually replace the file on all Agents in the cluster. From now on, you can force the synchronization of this file via Cube.

See also [Synchronizing data between DataMiner Agents](xref:Synchronizing_data_between_DataMiner_Agents)

### Fixes

*No fixes have been added yet.*
