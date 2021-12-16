v1alpha1.extension_repo('rails', url='file://{}'.format(config.main_dir))
v1alpha1.extension('rails-db', repo_name='rails', repo_path='rails-db', args=['--database', 'postgres'])
v1alpha1.extension('rails', repo_name='rails', repo_path='rails')

load('./rails/Tiltfile', 'rails_app')
rails_app('blorgh', '--database=postgresql')
