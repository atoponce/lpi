lpi
===

Disclaimer
----------

The purpose of this repository is to allow me to create paper quizzes and
exams for students of the University of Utah LPI courses provided by Guru
Labs. The quiz and exam sources are encrypted, to prevent students from
cheating. The repository exists, so I can develop the class from multiple
computers.

Sample
------

The YAML files are in the following syntax:
    
    quiz:
        - question:
            source: none
            text: What is the full path of the file used to ensure filesystems are mounted during boot?
            type: respond
            answers:
                - correct: /etc/fstab
        - question:
            source: none
            text: The "/etc/fstab" file is used to esure that filesystems are mounted on boot.
            type: truefalse
            answers:
                - correct: true
        - question:
            source: none
            text: Which file ensures that filesystems are mounted on boot?
            type: pickone
            answers:
                - correct: /etc/fstab
                - incorrect: /etc/mtab
                - incorrect: /etc/crypttab
                - incorrect: /etc/crontab
        - question:
            source: none
            text: Which of the following commands can unmount the "/dev/sda1" filesystem from "/mnt"? Select all that apply.
            type: pickmany
            answers:
                - correct: umount /dev/sda1
                - correct: umount /mnt
                - incorrect: unmount /dev/sda1
                - incorrect: unmount /mnt
                - incorrect: mount -U /dev/sda1 /mnt

Building
--------

A Python script will eventually be included.
