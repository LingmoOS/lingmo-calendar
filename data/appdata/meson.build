appdata_conf = configuration_data()
appdata_conf.set('appid', application_id)
appdata = i18n.merge_file(
  input: configure_file(
    input: files('org.lingmo.Calendar.appdata.xml.in.in'),
    output: 'org.lingmo.Calendar.appdata.xml.in',
    configuration: appdata_conf
  ),
  output: '@0@.appdata.xml'.format(application_id),
  po_dir: po_dir,
  install: true,
  install_dir: calendar_datadir / 'metainfo'
)
