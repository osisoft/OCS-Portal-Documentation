---
uid: PISystemconnections
---

# PI System Connections

You can use the OCS Connections feature to create a PI System connection and then stream data from your on-prem PI System to the desired namespace in OCS.

To create a data connection, perform the following steps:

  1. At the **Connections** page, click the **Type** field, then select **PI System**.

  2. Click the **Namespace** drop-down arrow and select the OCS namespace that you want your PI System data to be transferred into.

  3. Click **Add Connection**.

  4. In the **Add PI System Connection** window, enter a name and description for the new connection, then click **Next**.

  5. Verify the namespace is correct, then click **Save**.
  
      **Result:** The **Download Installation Kit** window opens.   
      
      **Note:**Each connection you create requires a new installation of the **PI to OSC agent**.                      |

  6. Download and install the latest version of the **PI to OCS Agent**. For instructions, see the *PI to OCS User Guide*.    
  
  7. Verify that **Registered** appears next to the **Data Source Status** field in the **Details** pane.                       
  
  **NOTE:** It can take a few minutes after installing the PI to OCS Agent for a data source to be registered. Once your data source is registered, you are ready to create a data transfer. 
    
  8. Select the connection on the **Connections** page, then click **Add PI Point Transfer**.

      **Result:** The **Add PI Point Transfer** window opens.       
      
  9.  **Optional:** Click the **Advanced** button to display more search fields (**Descriptor**, **Engineering Units**, **Point Type**, **Extended Descriptor**, and **Location Codes**).                                                    
  
  **NOTE:** To use the advanced search features, you need to have version 1.3.0.0 or higher of the agent.

10. In the **Add PI Point Transfer** window, define your query criteria by specifying values in one or more of the following fields: 

        **Name** (alias for tag attribute): Enter part or all of a   point name

        **Point Source**: Enter part or all of the point source name 

    **Descriptor**: Enter a part or all of a point\'s            description.

    **Engineering Units**: Enter a unit of measurement.          

    **Point Type**: Select one of the point types (Float32,     Float64, Int16, Int32, Digital, Timestamp or String) from    the drop-down list.

    **Extended Descriptor**: Enter a part or all of a point\'s   extended description.

    **Location Codes**: Enter up to five location code values    (1-9) in this field.                                         

  11. **Optional:**Click the **Basic** button to hide advanced search fields.

  12. **Optional:**To remove advanced filters from the search criteria, click **x** on the field label.

  13. Click the **Search** button to execute your query.           

      **Result:** Search results are listed in the **PI Points     Found** list box.                                            

  14. Select the desired PI points for the transfer, then click**Add**.                                                
  
      **Note:** You can create multiple queries and add additional PI points to your PI points transfer.                        |

  15. Enter a date and start time in the **Historical Start Time** fields.                                                      
      **Note:** No data prior to the time entered in this field  will be backfilled and written to SDS.                       |

  16. Click **Add Transfer** to save the transfer.                 |

      **Result:** Transfer details appear in the **Data Transfer** section of the **Details** tab.                              |

  17. In the **Data Transfer** section, click the **Start** button, then click **Start** in the **Start Transfer?** message box to begin streaming PI point data into the selected namespace in OCS.

**NOTE:** To interrupt or stop the transfer, click the **Stop** button in the **Data Transfer** section.

To edit an existing connection, follow these steps:

  1. Select an existing connection in the **Connections** page, then click **Edit Connection**.

  2. In the **Edit** window, edit the connection\'s name and description, then click **Next**.

  3. In the **Review** panel, click **Save**.

To delete an existing connection, follow these steps:

  1. Select an existing connection in the **Connections** page.

  2. **Optional:** If the connection has a data transfer in progress, you must stop the transfer before it can be removed. To stop the transfer, click the **Stop** button in the **Data Transfer** section of the **Details** pane.

  3. On the **Connections** page, click **Remove Connection**, then click **Remove**.

