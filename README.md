# AWS-CloudWatch-Monitoring
Created an AWS CloudWatch project to monitor EC2 instances, track CPU utilization, view logs, and configure monitoring alarms. Learned how to monitor AWS resources and identify performance issues using CloudWatch.

## 📌 Project Overview

This project demonstrates how to create an **Amazon CloudWatch Alarm** to monitor CPU utilization of an Amazon EC2 instance.

The CloudWatch alarm monitors the `CPUUtilization` metric. When the average CPU utilization exceeds **30%**, the alarm automatically changes its state from `OK` to `ALARM`.

## 🎯 Project Objectives

- Monitor EC2 instance CPU utilization.
- Configure CloudWatch metrics.
- Create a CloudWatch alarm.
- Set a CPU utilization threshold of 30%.
- Detect high CPU usage.
- Understand CloudWatch alarm states.

## 🛠️ AWS Services Used

| AWS Service | Purpose |
|---|---|
| Amazon EC2 | Virtual server |
| Amazon CloudWatch | CPU utilization monitoring |
| CloudWatch Alarm | Detect high CPU usage |
| AWS CLI | Configure AWS resources |

## 🏗️ Project Architecture

```text
       ┌──────────────────┐
       │    Amazon EC2    │
       │     MyServer     │
       └────────┬─────────┘
                │
                │ CPU Utilization
                ▼
       ┌──────────────────┐
       │ Amazon CloudWatch│
       │  CPUUtilization  │
       └────────┬─────────┘
                │
                │ CPU > 30%
                ▼
       ┌──────────────────┐
       │ CloudWatch Alarm │
       │   ALARM State    │
       └──────────────────┘
```

## 🚀 Implementation Steps

## Step 1: Open Amazon CloudWatch

1. Log in to the **AWS Management Console**.
2. Search for **CloudWatch** in the search bar.
3. Click **CloudWatch – Monitor Resources and Applications**.
4. Verify that the AWS Region is set to **Europe (Stockholm)**.
5. Open the CloudWatch service.

**Description:**

I accessed Amazon CloudWatch through the AWS Management Console to start configuring an alarm for monitoring EC2 CPU utilization.
![Step 1 - Open Amazon CloudWatch](screenshots/1.png)

---

## Step 2: Open CloudWatch Alarms

1. In the left-side menu of the CloudWatch Dashboard, click **Alarms**.
2. The CloudWatch Alarms section will open.
3. From this section, you can create and manage alarms for your EC2 instance.
4. Click **Create alarm** to start configuring a CPU utilization alarm.

**Description:**

I navigated to the Alarms section in Amazon CloudWatch to create an alarm for monitoring my EC2 instance's CPU utilization.
![Step 2 - CloudWatch Alarms](screenshots/2.png)

---

## Step 2: Click on Create Alarm

1. In the left-side menu of the CloudWatch Dashboard, click **Alarms**.
2. The CloudWatch Alarms page will open.
3. Click the **Create alarm** button in the top-right corner.
4. The alarm creation page will open.

**Description:**

I opened the CloudWatch Alarms section and clicked the **Create alarm** button to start creating an alarm for monitoring EC2 CPU utilization.
![Step 2 - Create CloudWatch Alarm](screenshots/2.png)

---

## Step 3: Create CloudWatch Alarm

1. On the CloudWatch Alarms page, locate the **Create alarm** button.
2. Click **Create alarm** in the top-right corner.
3. This will open the alarm configuration page.

**Description:**

I clicked the **Create alarm** button to start creating a new CloudWatch alarm for monitoring EC2 CPU utilization.
![Step 3 - Create CloudWatch Alarm](screenshots/3.png)

---

## Step 4: Specify Metric and Conditions

1. On the **Create alarm** page, select **Metrics** under Data source.
2. Under Type, keep **Classic** selected.
3. In the Metric section, click **Select metric**.
4. This will open the metric selection page.
5. Select the EC2 `CPUUtilization` metric for your instance.

**Description:**

I selected Metrics as the data source and Classic as the metric type. Then I clicked **Select metric** to choose the EC2 CPU utilization metric for creating the CloudWatch alarm.
![Step 4 - Specify Metric and Conditions](screenshots/4.png)

---

## Step 5: Select EC2 Metrics

1. On the **Select metric** page, locate the **EC2** category.
2. Click **EC2** to view the available EC2 metrics.
3. Select the **Per-Instance Metrics** option on the next page.
4. Find your EC2 instance named **MyServer**.

**Description:**

I selected the EC2 category from the CloudWatch metric selection page to access the available metrics for my EC2 instance.
![Step 5 - Select EC2 Metrics](screenshots/5.png)

---

## Step 6: Select Per-Instance Metrics

1. On the EC2 metrics page, click **Per-Instance Metrics**.
2. The list of available EC2 instance metrics will appear.
3. Locate your instance named **MyServer**.
4. Select the required CPU utilization metric in the next step.

**Description:**

I selected **Per-Instance Metrics** to view the monitoring metrics associated with my EC2 instance.
![Step 6 - Per-Instance Metrics](screenshots/6.png)

---






