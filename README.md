name: Metrics

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:
  push:
    branches:
      - main

jobs:
  github-metrics:
    runs-on: ubuntu-latest

    permissions:
      contents: write

    steps:
      - uses: lowlighter/metrics@latest
        with:
          token: ${{ secrets.METRICS_TOKEN }}

          user: Himanshu2800
          template: classic
          config_timezone: Asia/Kolkata

          base: header, activity, community, repositories

          plugin_isocalendar: yes
          plugin_isocalendar_duration: full-year

          plugin_languages: yes
          plugin_languages_limit: 8
