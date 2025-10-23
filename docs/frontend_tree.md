```bash
lib/
├── core/
│   ├── di/                          # Dependency Injection
│   │   ├── service_locator.dart
│   │   ├── dependency_injector.dart
│   │   └── service_providers.dart
│   ├── constants/
│   │   ├── app_colors.dart
│   │   ├── app_images.dart
│   │   ├── app_strings.dart
│   │   ├── app_styles.dart
│   │   ├── app_constants.dart
│   │   ├── delivery_constants.dart
│   │   └── api_endpoints.dart
│   ├── errors/
│   │   ├── exceptions.dart
│   │   ├── failures.dart
│   │   ├── error_handler.dart
│   │   ├── error_logger.dart
│   │   └── error_mapper.dart
│   ├── network/
│   │   ├── api_client.dart
│   │   ├── api_constants.dart
│   │   ├── api_interceptor.dart
│   │   ├── dio_security_config.dart
│   │   ├── connectivity_checker.dart
│   │   ├── request_retry.dart
│   │   └── api_response.dart
│   ├── security/
│   │   ├── biometric_auth.dart
│   │   ├── encryption_service.dart
│   │   ├── app_integrity_checker.dart
│   │   ├── secure_storage.dart
│   │   ├── transaction_signer.dart
│   │   ├── threat_detector.dart
│   │   ├── certificate_pinner.dart
│   │   └── security_scanner.dart
│   ├── themes/
│   │   ├── app_theme.dart
│   │   ├── color_palette.dart
│   │   ├── text_themes.dart
│   │   ├── button_themes.dart
│   │   ├── input_themes.dart
│   │   └── dark_theme.dart
│   ├── utils/
│   │   ├── ar_utils.dart
│   │   ├── nft_utils.dart
│   │   ├── mpesa_utils.dart
│   │   ├── image_utils.dart
│   │   ├── validators.dart
│   │   ├── date_utils.dart
│   │   ├── location_utils.dart
│   │   ├── delivery_calculator.dart
│   │   ├── price_formatter.dart
│   │   ├── file_picker_utils.dart
│   │   ├── permissions_handler.dart
│   │   ├── debouncer.dart
│   │   ├── logger.dart
│   │   └── platform_detector.dart
│   ├── widgets/
│   │   ├── common/
│   │   │   ├── custom_app_bar.dart
│   │   │   ├── custom_button.dart
│   │   │   ├── custom_text_field.dart
│   │   │   ├── loading_indicator.dart
│   │   │   ├── error_widget.dart
│   │   │   ├── empty_state.dart
│   │   │   ├── retry_button.dart
│   │   │   └── shimmer_effect.dart
│   │   ├── product/
│   │   │   ├── product_card.dart
│   │   │   ├── product_grid.dart
│   │   │   ├── product_carousel.dart
│   │   │   ├── featured_products.dart
│   │   │   └── product_skeleton.dart
│   │   ├── ar/
│   │   │   ├── ar_viewer.dart
│   │   │   ├── ar_controls.dart
│   │   │   ├── ar_loading_indicator.dart
│   │   │   ├── ar_placement_guide.dart
│   │   │   └── ar_error_boundary.dart
│   │   ├── security/
│   │   │   ├── biometric_prompt.dart
│   │   │   ├── security_badge.dart
│   │   │   ├── verified_checkmark.dart
│   │   │   ├── security_shield.dart
│   │   │   └── security_overlay.dart
│   │   └── delivery/
│   │       ├── delivery_tracker.dart
│   │       ├── delivery_pricing_card.dart
│   │       ├── address_selector.dart
│   │       ├── courier_rating.dart
│   │       ├── live_tracking_map.dart
│   │       └── delivery_timeline.dart
│   └── state_management/
│       ├── app_bloc_observer.dart
│       ├── base_cubit.dart
│       ├── base_state.dart
│       └── state_utils.dart
├── features/
│   ├── auth/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── auth_remote_data_source.dart
│   │   │   │   ├── auth_local_data_source.dart
│   │   │   │   └── auth_secure_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── auth_model.dart
│   │   │   │   ├── user_model.dart
│   │   │   │   └── session_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── auth_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── user_mapper.dart
│   │   │       └── auth_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── auth_entity.dart
│   │   │   │   ├── user_entity.dart
│   │   │   │   └── session_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── auth_repository.dart
│   │   │   └── usecases/
│   │   │       ├── login.dart
│   │   │       ├── signup.dart
│   │   │       ├── logout.dart
│   │   │       ├── get_user.dart
│   │   │       ├── verify_biometrics.dart
│   │   │       ├── change_password.dart
│   │   │       ├── reset_password.dart
│   │   │       └── validate_session.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── auth_cubit.dart
│   │       │   └── auth_state.dart
│   │       ├── pages/
│   │       │   ├── login_screen.dart
│   │       │   ├── signup_screen.dart
│   │       │   ├── onboarding_screen.dart
│   │       │   ├── verify_phone_screen.dart
│   │       │   ├── biometric_setup_screen.dart
│   │       │   ├── security_settings_screen.dart
│   │       │   └── forgot_password_screen.dart
│   │       └── widgets/
│   │           ├── login_form.dart
│   │           ├── signup_form.dart
│   │           ├── social_auth_buttons.dart
│   │           ├── biometric_toggle.dart
│   │           ├── security_level_indicator.dart
│   │           ├── password_strength_meter.dart
│   │           └── session_timeout_warning.dart
│   ├── marketplace/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── marketplace_remote_data_source.dart
│   │   │   │   ├── marketplace_local_data_source.dart
│   │   │   │   └── marketplace_cache_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── product_model.dart
│   │   │   │   ├── shop_model.dart
│   │   │   │   ├── category_model.dart
│   │   │   │   └── search_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── marketplace_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── product_mapper.dart
│   │   │       ├── shop_mapper.dart
│   │   │       └── category_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── product_entity.dart
│   │   │   │   ├── shop_entity.dart
│   │   │   │   ├── category_entity.dart
│   │   │   │   └── search_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── marketplace_repository.dart
│   │   │   └── usecases/
│   │   │       ├── get_products.dart
│   │   │       ├── get_product_detail.dart
│   │   │       ├── create_product_listing.dart
│   │   │       ├── update_product_listing.dart
│   │   │       ├── delete_product_listing.dart
│   │   │       ├── search_products.dart
│   │   │       ├── filter_products.dart
│   │   │       ├── get_categories.dart
│   │   │       └── get_trending_products.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── marketplace_cubit.dart
│   │       │   ├── marketplace_state.dart
│   │       │   ├── search_cubit.dart
│   │       │   └── search_state.dart
│   │       ├── pages/
│   │       │   ├── home_screen.dart
│   │       │   ├── product_detail_screen.dart
│   │       │   ├── create_listing_screen.dart
│   │       │   ├── search_screen.dart
│   │       │   ├── categories_screen.dart
│   │       │   ├── discover_screen.dart
│   │       │   ├── shop_profile_screen.dart
│   │       │   └── edit_listing_screen.dart
│   │       └── widgets/
│   │           ├── product_grid.dart
│   │           ├── product_carousel.dart
│   │           ├── search_bar.dart
│   │           ├── category_filter.dart
│   │           ├── featured_products.dart
│   │           ├── trending_sellers.dart
│   │           ├── shop_header.dart
│   │           ├── product_image_gallery.dart
│   │           └── category_chips.dart
│   ├── ar_viewer/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── ar_remote_data_source.dart
│   │   │   │   ├── ar_local_data_source.dart
│   │   │   │   └── ar_cache_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── ar_model.dart
│   │   │   │   ├── ar_session_model.dart
│   │   │   │   └── ar_anchor_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── ar_repository_impl.dart
│   │   │   └── mappers/
│   │   │       └── ar_model_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── ar_entity.dart
│   │   │   │   ├── ar_session_entity.dart
│   │   │   │   └── ar_anchor_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── ar_repository.dart
│   │   │   └── usecases/
│   │   │       ├── load_ar_model.dart
│   │   │       ├── capture_ar_snapshot.dart
│   │   │       ├── save_ar_session.dart
│   │   │       ├── load_ar_session.dart
│   │   │       └── detect_ar_surface.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── ar_cubit.dart
│   │       │   └── ar_state.dart
│   │       ├── pages/
│   │       │   ├── ar_view_screen.dart
│   │       │   ├── ar_gallery_screen.dart
│   │       │   └── ar_session_screen.dart
│   │       └── widgets/
│   │           ├── ar_controls.dart
│   │           ├── ar_loading_indicator.dart
│   │           ├── ar_placement_guide.dart
│   │           ├── ar_error_boundary.dart
│   │           ├── ar_snapshot_button.dart
│   │           └── ar_environment_scanner.dart
│   ├── nft/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── nft_remote_data_source.dart
│   │   │   │   ├── nft_blockchain_data_source.dart
│   │   │   │   └── nft_local_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── nft_model.dart
│   │   │   │   ├── nft_metadata_model.dart
│   │   │   │   └── nft_transaction_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── nft_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── nft_mapper.dart
│   │   │       └── nft_metadata_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── nft_entity.dart
│   │   │   │   ├── nft_metadata_entity.dart
│   │   │   │   └── nft_transaction_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── nft_repository.dart
│   │   │   └── usecases/
│   │   │       ├── mint_nft.dart
│   │   │       ├── transfer_nft.dart
│   │   │       ├── get_nft_detail.dart
│   │   │       ├── verify_nft_ownership.dart
│   │   │       ├── get_my_nfts.dart
│   │   │       └── get_nft_history.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── nft_cubit.dart
│   │       │   └── nft_state.dart
│   │       ├── pages/
│   │       │   ├── nft_detail_screen.dart
│   │       │   ├── mint_nft_screen.dart
│   │       │   ├── my_nfts_screen.dart
│   │       │   ├── nft_gallery_screen.dart
│   │       │   └── nft_transfer_screen.dart
│   │       └── widgets/
│   │           ├── nft_card.dart
│   │           ├── nft_metadata_view.dart
│   │           ├── nft_transaction_history.dart
│   │           ├── nft_ownership_badge.dart
│   │           └── nft_minting_progress.dart
│   ├── delivery/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── delivery_remote_data_source.dart
│   │   │   │   ├── delivery_local_data_source.dart
│   │   │   │   └── delivery_gps_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── delivery_model.dart
│   │   │   │   ├── address_model.dart
│   │   │   │   ├── courier_model.dart
│   │   │   │   ├── pricing_model.dart
│   │   │   │   └── tracking_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── delivery_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── delivery_mapper.dart
│   │   │       ├── address_mapper.dart
│   │   │       └── courier_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── delivery_entity.dart
│   │   │   │   ├── address_entity.dart
│   │   │   │   ├── courier_entity.dart
│   │   │   │   ├── pricing_entity.dart
│   │   │   │   └── tracking_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── delivery_repository.dart
│   │   │   └── usecases/
│   │   │       ├── calculate_delivery_cost.dart
│   │   │       ├── track_delivery.dart
│   │   │       ├── get_delivery_history.dart
│   │   │       ├── schedule_delivery.dart
│   │   │       ├── rate_courier.dart
│   │   │       ├── find_nearby_couriers.dart
│   │   │       ├── update_delivery_address.dart
│   │   │       └── cancel_delivery.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── delivery_cubit.dart
│   │       │   └── delivery_state.dart
│   │       ├── pages/
│   │       │   ├── delivery_tracking_screen.dart
│   │       │   ├── delivery_options_screen.dart
│   │       │   ├── address_management_screen.dart
│   │       │   ├── courier_selection_screen.dart
│   │       │   ├── delivery_pricing_screen.dart
│   │       │   ├── delivery_history_screen.dart
│   │       │   └── live_tracking_screen.dart
│   │       └── widgets/
│   │           ├── delivery_timeline.dart
│   │           ├── live_tracking_map.dart
│   │           ├── delivery_status_badge.dart
│   │           ├── courier_card.dart
│   │           ├── pricing_calculator.dart
│   │           ├── address_form.dart
│   │           ├── delivery_progress_bar.dart
│   │           └── estimated_arrival.dart
│   ├── checkout/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── checkout_remote_data_source.dart
│   │   │   │   ├── checkout_local_data_source.dart
│   │   │   │   └── checkout_cache_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── cart_model.dart
│   │   │   │   ├── order_model.dart
│   │   │   │   ├── checkout_model.dart
│   │   │   │   └── promo_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── checkout_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── cart_mapper.dart
│   │   │       ├── order_mapper.dart
│   │   │       └── checkout_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── cart_entity.dart
│   │   │   │   ├── order_entity.dart
│   │   │   │   ├── checkout_entity.dart
│   │   │   │   └── promo_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── checkout_repository.dart
│   │   │   └── usecases/
│   │   │       ├── add_to_cart.dart
│   │   │       ├── remove_from_cart.dart
│   │   │       ├── get_cart_items.dart
│   │   │       ├── create_order.dart
│   │   │       ├── apply_promo_code.dart
│   │   │       ├── validate_checkout.dart
│   │   │       ├── calculate_totals.dart
│   │   │       └── update_cart_quantity.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── checkout_cubit.dart
│   │       │   └── checkout_state.dart
│   │       ├── pages/
│   │       │   ├── cart_screen.dart
│   │       │   ├── checkout_screen.dart
│   │       │   ├── order_summary_screen.dart
│   │       │   ├── order_confirmation_screen.dart
│   │       │   ├── order_history_screen.dart
│   │       │   └── order_details_screen.dart
│   │       └── widgets/
│   │           ├── cart_item.dart
│   │           ├── order_summary_card.dart
│   │           ├── promo_code_field.dart
│   │           ├── checkout_stepper.dart
│   │           ├── order_timeline.dart
│   │           ├── payment_method_selector.dart
│   │           └── order_status_tracker.dart
│   ├── payment/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── payment_remote_data_source.dart
│   │   │   │   ├── payment_secure_data_source.dart
│   │   │   │   └── payment_mpesa_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── payment_model.dart
│   │   │   │   ├── mpesa_model.dart
│   │   │   │   └── transaction_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── payment_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── payment_mapper.dart
│   │   │       └── transaction_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── payment_entity.dart
│   │   │   │   ├── mpesa_entity.dart
│   │   │   │   └── transaction_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── payment_repository.dart
│   │   │   └── usecases/
│   │   │       ├── initiate_payment.dart
│   │   │       ├── confirm_payment.dart
│   │   │       ├── get_payment_history.dart
│   │   │       ├── process_mpesa_payment.dart
│   │   │       ├── verify_transaction.dart
│   │   │       └── refund_payment.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── payment_cubit.dart
│   │       │   └── payment_state.dart
│   │       ├── pages/
│   │       │   ├── payment_methods_screen.dart
│   │       │   ├── mpesa_payment_screen.dart
│   │       │   ├── payment_processing_screen.dart
│   │       │   ├── payment_success_screen.dart
│   │       │   ├── payment_failed_screen.dart
│   │       │   └── transaction_history_screen.dart
│   │       └── widgets/
│   │           ├── mpesa_payment_form.dart
│   │           ├── payment_summary.dart
│   │           ├── payment_security_badge.dart
│   │           ├── transaction_item.dart
│   │           └── payment_method_card.dart
│   ├── chat/
│   │   ├── data/
│   │   │   ├── datasources/
│   │   │   │   ├── chat_remote_data_source.dart
│   │   │   │   ├── chat_local_data_source.dart
│   │   │   │   └── chat_socket_data_source.dart
│   │   │   ├── models/
│   │   │   │   ├── chat_model.dart
│   │   │   │   ├── message_model.dart
│   │   │   │   └── conversation_model.dart
│   │   │   ├── repositories/
│   │   │   │   └── chat_repository_impl.dart
│   │   │   └── mappers/
│   │   │       ├── chat_mapper.dart
│   │   │       ├── message_mapper.dart
│   │   │       └── conversation_mapper.dart
│   │   ├── domain/
│   │   │   ├── entities/
│   │   │   │   ├── chat_entity.dart
│   │   │   │   ├── message_entity.dart
│   │   │   │   └── conversation_entity.dart
│   │   │   ├── repositories/
│   │   │   │   └── chat_repository.dart
│   │   │   └── usecases/
│   │   │       ├── get_chats.dart
│   │   │       ├── send_message.dart
│   │   │       ├── delete_message.dart
│   │   │       ├── mark_as_read.dart
│   │   │       ├── get_conversation.dart
│   │   │       └── start_conversation.dart
│   │   └── presentation/
│   │       ├── cubit/
│   │       │   ├── chat_cubit.dart
│   │       │   └── chat_state.dart
│   │       ├── pages/
│   │       │   ├── chat_list_screen.dart
│   │       │   ├── chat_detail_screen.dart
│   │       │   ├── conversation_screen.dart
│   │       │   └── new_chat_screen.dart
│   │       └── widgets/
│   │           ├── chat_bubble.dart
│   │           ├── message_input.dart
│   │           ├── chat_list_tile.dart
│   │           ├── typing_indicator.dart
│   │           ├── message_status.dart
│   │           └── chat_attachment_picker.dart
│   └── profile/
│       ├── data/
│       │   ├── datasources/
│       │   │   ├── profile_remote_data_source.dart
│       │   │   ├── profile_local_data_source.dart
│       │   │   └── profile_secure_data_source.dart
│       │   ├── models/
│       │   │   ├── profile_model.dart
│       │   │   ├── tier_model.dart
│       │   │   ├── analytics_model.dart
│       │   │   └── settings_model.dart
│       │   ├── repositories/
│       │   │   └── profile_repository_impl.dart
│       │   └── mappers/
│       │       ├── profile_mapper.dart
│       │       ├── tier_mapper.dart
│       │       └── analytics_mapper.dart
│       ├── domain/
│       │   ├── entities/
│       │   │   ├── profile_entity.dart
│       │   │   ├── tier_entity.dart
│       │   │   ├── analytics_entity.dart
│       │   │   └── settings_entity.dart
│       │   ├── repositories/
│       │   │   └── profile_repository.dart
│       │   └── usecases/
│       │       ├── get_profile.dart
│       │       ├── update_profile.dart
│       │       ├── upgrade_tier.dart
│       │       ├── get_analytics.dart
│       │       ├── update_settings.dart
│       │       ├── delete_account.dart
│       │       └── export_data.dart
│       └── presentation/
│           ├── cubit/
│           │   ├── profile_cubit.dart
│           │   └── profile_state.dart
│           ├── pages/
│           │   ├── profile_screen.dart
│           │   ├── edit_profile_screen.dart
│           │   ├── tier_upgrade_screen.dart
│           │   ├── settings_screen.dart
│           │   ├── analytics_screen.dart
│           │   ├── security_center_screen.dart
│           │   ├── help_support_screen.dart
│           │   └── about_screen.dart
│           └── widgets/
│               ├── profile_header.dart
│               ├── tier_badge.dart
│               ├── settings_tile.dart
│               ├── stats_card.dart
│               ├── security_status.dart
│               ├── analytics_chart.dart
│               └── profile_quick_actions.dart
├── app/
│   ├── cubit/
│   │   ├── app_cubit.dart
│   │   ├── app_state.dart
│   │   └── app_event_handler.dart
│   ├── pages/
│   │   ├── main_screen.dart
│   │   ├── splash_screen.dart
│   │   ├── error_screen.dart
│   │   ├── maintenance_screen.dart
│   │   └── update_required_screen.dart
│   └── widgets/
│       ├── bottom_nav_bar.dart
│       ├── custom_drawer.dart
│       ├── floating_action_button.dart
│       ├── app_update_dialog.dart
│       ├── network_status_bar.dart
│       └── app_lifecycle_handler.dart
├── shared/
│   ├── services/
│   │   ├── push_notification_service.dart
│   │   ├── deep_link_service.dart
│   │   ├── background_fetch_service.dart
│   │   ├── analytics_service.dart
│   │   ├── crashlytics_service.dart
│   │   ├── performance_monitoring_service.dart
│   │   └── app_review_service.dart
│   ├── mixins/
│   │   ├── validation_mixin.dart
│   │   ├── permission_mixin.dart
│   │   ├── loading_mixin.dart
│   │   ├── error_mixin.dart
│   │   └── keyboard_mixin.dart
│   └── extensions/
│       ├── string_extensions.dart
│       ├── datetime_extensions.dart
│       ├── list_extensions.dart
│       ├── context_extensions.dart
│       └── num_extensions.dart
└── main.dart