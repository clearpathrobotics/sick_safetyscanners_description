sick_safetyscanners_description
=====================================

This package contains the necessary STL and URDF files to easily add the Sick Outdoor Scan 3, Micro Scan 3, and
Nano Scan 3 safety lidars to your robot.

A macro is defined for each included sensor.  To add it to your URDF simply `include` the file, and insert the
macro.  For example:

    <xacro:include filename="$(find sick_safetyscanners_description)/urdf/outdoorscan3.urdf.xacro" />
    <xacro:outdoorscan3 prefix="front" parent_link="front_mount" topic="front/scan">
      <origin xyz="0 0 0" rpy="0 0 0" />
    </xacro:outdoorscan3>
